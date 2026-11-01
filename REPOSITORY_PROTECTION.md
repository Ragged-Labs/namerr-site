# Protecting the Namerr website repository

**Important:** GitHub rulesets are server-side repository settings. A JSON file committed to the repository is a **configuration template only** and does **not** activate protection. The GitHub connection used to prepare this website can read rulesets but does not expose a ruleset-creation/admin-write operation. A repository administrator must apply the settings directly in GitHub.

## Recommended active ruleset

Repository: `Ragged-Labs/namerr-site`

In GitHub, open **Settings → Rules → Rulesets → New ruleset → New branch ruleset**.

- **Ruleset name:** `Protect website main - pull requests and history`.
- **Enforcement:** Active.
- **Target branches:** include the default branch (`main`).
- **Restrict deletions:** On.
- **Block force pushes:** On.
- **Require a pull request before merging:** On.
- **Required approvals:** **0** for the current single-maintainer setup. This requires a PR without locking the owner into obtaining a second human's approval. Increase to 1 when another authorised reviewer is available.
- **Require linear history:** On. Merge website pull requests with **Squash and merge**; do not use merge commits.
- **Require review-thread resolution:** Optional; can be enabled after collaborators join.
- **Require status checks:** Leave Off until a stable, lightweight website check is configured and observed successfully. Do **not** require a non-existent job or a GitHub Pages post-merge deployment check.
- **Require signed commits:** Leave Off until the signing scheme for the GitHub application is tested.
- **Bypass:** Prefer no permanent bypass, or narrowly limit to a trusted administrator for emergencies. An administrator can manage the ruleset itself.

Select **Create** and verify that the ruleset is **Active** and targets `main`.

Direct entrypoint: https://github.com/Ragged-Labs/namerr-site/settings/rules

## Verify ruleset is actually active

1. Confirm the rule is visible in Settings → Rules → Rulesets with status Active.
2. Confirm `main` displays the protection rules and cannot be force-pushed or deleted by ordinary contributors.
3. Merge future changes through PRs (the website's GitHub Pages branch publishing remains independent of custom Actions).
4. Verify no unexpected rules require paid features or disable the existing automated GitHub Pages publishing.
5. An active ruleset should appear at the repository rulesets API endpoint: `GET https://api.github.com/repos/Ragged-Labs/namerr-site/rulesets`.

The checked-in API-ready template is in [rulesets/main-protection.json](rulesets/main-protection.json). It is not executed or auto-imported by GitHub.

## Site safety during prelaunch

- Coming Soon is the public `main` website.
- Full website v1 is preserved in `archive/website-v1-before-coming-soon`.
- The richer branding/donation proposal is still in draft PR #5; **do not merge it directly over the Coming Soon page** without a deliberate launch decision.
- There is no active downloadable package, payment destination or Bitcoin receiving address.
- The application repositories and existing five-hour engineering automation are out of scope.
