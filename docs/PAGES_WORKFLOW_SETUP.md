# Namerr GitHub Pages — serialized publishing

## Safe cutover

This repository contains one custom workflow: `.github/workflows/publish-pages.yml`.

1. **Do not enable two Pages publishers concurrently.** The workflow checks the live Pages build type and deliberately skips deployment while the source is `Deploy from a branch`.
2. Once the workflow is merged to `main`, open [Settings → Pages](https://github.com/Ragged-Labs/namerr-site/settings/pages).
3. Under **Build and deployment → Source**, choose **GitHub Actions**. GitHub may suggest a template; **do not create a second template**. Use the existing `Publish Namerr website` workflow.
4. Open [Actions → Publish Namerr website](https://github.com/Ragged-Labs/namerr-site/actions/workflows/publish-pages.yml). Choose **Run workflow → main → Run workflow** once.
5. Confirm the `build` and `deploy` jobs both succeed and that https://ragged-labs.github.io/namerr-site/ shows the latest site.
6. Future pushes affecting HTML, assets or sitemap automatically use this workflow. You can also re-run it manually when needed; avoid repeated manual reruns.

## Concurrency and efficiency

- `concurrency.group: namerr-pages-production` serializes all publish runs.
- `cancel-in-progress: false` protects an active deploy from interruption. By default, GitHub keeps only the latest pending run, replacing superseded pending runs.
- Preflight reads Pages source `build_type` and skips if the site still uses legacy branch publishing, avoiding a competing publisher.
- Output includes only static HTML, CSS, JS, image assets, sitemap and robots.txt, not the repository source/metadata.
- Build/asset checks are performed with Bash and require no dependency installation.
- The Pages artifact expires after **1 day**; this is independent of GitHub Actions caches and container image storage.
- This workflow does not build, modify or deploy the Namerr application.

## Troubleshooting

- If the build is successful but `deploy-pages` reports `due to in progress deployment`, open the relevant Actions run and check whether GitHub is still tracking an earlier deployment. Do not repeatedly create new runs.
- If `build` completes with the custom publishing-source notice and `deploy` is skipped, choose `GitHub Actions` in Settings → Pages (it is still configured for branch publishing).
- If the workflow cannot access Pages source state, verify Actions workflow token permissions allow Pages read/write, and that Pages has been enabled.
- Pages source configuration and repository rulesets are **GitHub repository settings**; committing this workflow does not alter the Pages setting.

## GitHub Actions reference

See https://docs.github.com/en/pages/getting-started-with-github-pages/using-custom-workflows-with-github-pages and https://docs.github.com/en/actions/how-tos/write-workflows/choose-when-workflows-run/control-workflow-concurrency.
