# Namerr — Coming Soon website

**Public site:** https://ragged-labs.github.io/namerr-site/

The public website for **Namerr**, a self-hosted media library organiser being developed by **RaggedLabs Media** (`raggedlabs.media`).

## Current publication state — 1 November 2026

- Public visitors see a branded **Coming Soon** page, focused on planned capabilities, project development status, and contact information.
- **No public application downloads, account registrations, donation payment links or wallet addresses are active.**
- Older `docs.html`, `roadmap.html`, `downloads.html`, `about.html` and `support.html` routes return visitors to the relevant section of the coming-soon home page. A public Privacy page and 404 page remain.
- The previous full multi-page website has been saved in branch `archive/website-v1-before-coming-soon`; the further draft About/donation concepts remain in PR #5.
- The official N logo is an exact copy of `Namerr-Docker-Icon.png` from the private application development repository.
- No custom website GitHub Actions workflow was added. Publication uses the existing GitHub Pages system.

## Developer and project repositories

- RaggedLabs Media: `raggedlabs.media` (brand domain).
- Organisation: https://github.com/Ragged-Labs.
- Website repository: `Ragged-Labs/namerr-site`.
- Official application repository: `Ragged-Labs/namerr` (private prelaunch placeholder, **not** a public release).
- Legacy development and current Docker image compatibility: `raggedred/emby_organiser_docker` (private).
- General enquiries: [contact@raggedlabs.media](mailto:contact@raggedlabs.media).
- X profile: https://x.com/namerrmedia.

## Site development

Open `index.html` locally or use a small static file server. Styles for the public launch hold live in `assets/coming-soon.css`. The former full site styles remain in `assets/site.css` for eventual reuse. Do not modify public app download links without confirming official release availability.

## Protect the repository

See [REPOSITORY_PROTECTION.md](REPOSITORY_PROTECTION.md) and the ruleset template at [docs/rulesets/main-protection.json](docs/rulesets/main-protection.json). **Committing ruleset JSON does not activate server-side GitHub protection**; a repository administrator must create an Active ruleset in Settings.

Security disclosures: [SECURITY.md](SECURITY.md). Before community launch, review [LAUNCH_CHECKLIST.md](LAUNCH_CHECKLIST.md).
