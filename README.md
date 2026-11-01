# Namerr — official website

This is the independent, **currently private prelaunch website** for **Namerr**, a self-hosted movie and TV organiser by **RaggedLabs Media** (`raggedlabs.media`).

## Current site status

- Static website preview implemented in HTML, CSS and vanilla JavaScript; **no framework, build or npm dependency required**.
- Official public application downloads **are not enabled yet**. The app repository and image publication must pass their separate public-launch checks before download links are activated.
- Donations **are not enabled yet**. Buy Me a Coffee (`/namerr`) and Bitcoin (BTC mainnet) are planned, with no receiving address, QR code or payment link until verified.
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

## Brand assets

The website uses `assets/namerr-logo-8dd16181.png`, an exact byte-for-byte copy of `Namerr-Docker-Icon.png` from `raggedred/emby_organiser_docker`. It is used for the header, favicon, Apple touch icon and Open Graph image. This replaces the original placeholder logo.

## Website logo cache control

All page templates reference the content-versioned official logo `assets/namerr-logo-8dd16181.png` (sha256-like prefix is the Git object SHA prefix). This is an exact copy of `Namerr-Docker-Icon.png` in the application repository and prevents browser caches from reusing previous logo URLs on Docs, Support, Roadmap and the homepage. The original logo path remains in Git for backward compatibility with older cached HTML.

## Developer identity, repositories and launch hold (1 November 2026)

- **RaggedLabs Media:** `raggedlabs.media`; public GitHub organisation `Ragged-Labs`; contact `contact@raggedlabs.media`.
- **Official product home:** `Ragged-Labs/namerr` is private and currently only a placeholder, **not** a public download source.
- **Website source:** `Ragged-Labs/namerr-site` is private prelaunch. Keep private until explicitly approved for public release.
- **Legacy app and Docker compatibility:** `raggedred/emby_organiser_docker` is private. Do not replace existing Docker image paths until migration and upgrades are validated.
- The parent brand-domain mention is not proof of a configured website. Do not set the site CNAME without domain ownership and DNS verification.

Read [DONATIONS_SETUP.md](DONATIONS_SETUP.md) for activation safeguards and [LAUNCH_CHECKLIST.md](LAUNCH_CHECKLIST.md) for the release gate. Never commit wallet recovery phrases, private keys, payment account credentials or access tokens.
