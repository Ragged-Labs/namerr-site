# Namerr — Coming Soon website

**Public site:** https://ragged-labs.github.io/namerr-site/

The public website for **Namerr**, a self-hosted media library organiser being developed by **RaggedLabs Media** (`raggedlabs.media`).

## Current publication state — 1 November 2026

- Public visitors see a branded **Coming Soon** page, focused on planned capabilities, project development status, and contact information.
- **No public application downloads, account registrations or Bitcoin wallet addresses are active.** A Support page now includes a proposed external Buy Me a Coffee link, with explicit recipient-verification warning.
- Older `docs.html`, `roadmap.html`, `downloads.html` and `about.html` routes return visitors to the relevant section of the coming-soon home page. `support.html` is a dedicated Support and Contact page with responsive equal-height contact cards. A public Privacy page and 404 page remain.
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

## Support link review

The external Buy Me a Coffee destination currently configured is `https://buymeacoffee.com/namerr`, based on the project owner’s specified prospective name. **The profile and payout recipient have not been independently verified.** Public copy explicitly instructs visitors to verify recipient identity before donating. Do not publish a Bitcoin receiving address without owner-supplied wallet verification.

## Planned UI gallery — source images

Four original AI-generated **31 October 2026 Namerr UI concept images** belong under `assets/previews/` (optimised WebP copies of the saved original PNGs). The index page already contains a responsive, lazy-loaded 2 × 2 gallery labelled **concept artwork, not shipped UI**.

| Web image path | Source Library image | UI subject |
|---|---|---|
| `assets/previews/tv-library-concept.webp` | `image-gen-1.png` | TV Shows library table |
| `assets/previews/guided-review-concept.webp` | `image-gen-2.png` | Guided Review workflow |
| `assets/previews/movie-library-concept.webp` | `image-gen-3.png` | Movies library poster grid |
| `assets/previews/change-preview-concept.webp` | `image-gen-4.png` | Review and Preview Changes |

**Do not merge the gallery PR until all four images are uploaded and their paths and display are tested.** This branch is intentionally held as a draft until the binary assets exist in the GitHub repository. The original PNGs are saved in the ChatGPT Movie Naming Tool image library; the web-optimised PNG-to-WebP bundle has been prepared separately for upload.
