# Namerr — official website

This is the independent public website for **Namerr**, a self-hosted TV and movie organiser by Ragged Labs.

## Current site status

- Static website preview implemented in HTML, CSS and vanilla JavaScript; **no framework, build or npm dependency required**.
- Official public application downloads **are not enabled yet**. The app repository and image publication must pass their separate public-launch checks before download links are activated.
- Donations **are not enabled yet**. Add a verified payment-provider URL before publishing an actionable donation button.
- Planned AI, Jellyfin, music, books, audiobooks and photos are clearly identified as roadmap items, not shipped product capabilities.
- The product's 5-hour application build automation and Docker release process are completely separate from this website.

## Local preview

Open `index.html` in a browser or serve this directory with `python -m http.server 8000`.

## Publish on GitHub Pages

1. Make `Ragged-Labs/namerr-site` **public** for GitHub Pages on a GitHub Free plan.
2. Merge the approved website pull request to `main`.
3. Repository **Settings → Pages → Build and deployment**: choose **Deploy from a branch**, then **main** and **/(root)**. Save.
4. Expected Pages URL: https://ragged-labs.github.io/namerr-site/ (confirm in Settings after publishing).
5. Optionally add a purchased custom domain later; do not add a `CNAME` file until ownership/DNS are verified.

See [LAUNCH_CHECKLIST.md](LAUNCH_CHECKLIST.md) for publication and donation/download activation gates.

## Editing

All links are relative to the repository site path, so Pages works without a custom domain. Update real public links only when tested. Avoid publishing private app repository URLs as working public downloads. No analytics, embeds, trackers, external fonts or cookies are installed by this site.
