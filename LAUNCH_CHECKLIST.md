# Public launch checklist — Namerr website

Website repository: `Ragged-Labs/namerr-site` (**private prelaunch**), separate from the private new product home `Ragged-Labs/namerr` and legacy development/compatibility repository `raggedred/emby_organiser_docker`.

## Website acceptance

- [ ] Review desktop, tablet and mobile layout, menu, keyboard navigation, contrast and anchor links.
- [ ] Confirm every feature is labelled **current** versus **planned** based on the published application release.
- [ ] Review website copy for brand and release accuracy.
- [ ] Open all pages and verify links, titles, favicon and custom 404.
- [ ] Publish website as public before enabling GitHub Pages on the GitHub Free plan.
- [ ] In Settings → Pages, set **Deploy from a branch** → **main** → **/(root)**.
- [ ] Confirm live page at `https://ragged-labs.github.io/namerr-site/`.
- [ ] Confirm HTTPS and mobile layout on the live domain.

## Public download gate — separate from website deployment

- [ ] Decide, document and approve product licensing (website MIT license does **not** license the separate application).
- [ ] Complete public-release security, package and installation validation.
- [ ] Confirm publicly accessible versioned Unraid/Docker installer and container image.
- [ ] Verify checksums/provenance and stable release notes for the public package.
- [ ] Validate clean install and legacy upgrade without changing legacy appdata paths or media mappings.
- [ ] Configure public app support/issue locations.
- [ ] Only then replace the informational download status with tested real release links.

## Donations — Buy Me a Coffee and Bitcoin

- [ ] Verify the exact Namerr Buy Me a Coffee creator account, payout recipient and fees. Proposed `buymeacoffee.com/namerr` is **unverified** and must not be linked yet.
- [ ] Verify ownership and payout destination before enabling any payment button.
- [ ] Confirm a dedicated Bitcoin mainnet BTC **public receiving address**, network and beneficiary; never publish wallet private keys or recovery phrases.
- [ ] Independently verify the exact displayed address and any QR code against the intended wallet.
- [ ] Explain public blockchain observability, irreversible transfers, fees, and relevant tax/accounting considerations.
- [ ] State that contributions are voluntary and do not buy feature priority or guaranteed support.
- [ ] Review [DONATIONS_SETUP.md](DONATIONS_SETUP.md) and obtain explicit public-activation approval.

## Brand and repository status

- [ ] Confirm use of RaggedLabs Media and `raggedlabs.media` on all public pages.
- [ ] Verify whether the parent brand domain has an actual live website before making it a clickable link.
- [ ] Keep `Ragged-Labs/namerr` private until the installer/release migration is complete.
- [ ] Keep `Ragged-Labs/namerr-site` private and do not republish Pages before explicit owner approval.

## Optional custom domain

- [ ] Check domain ownership/availability and purchase (a custom .media domain is not generally free).
- [ ] Point DNS at the GitHub Pages site per current GitHub instructions.
- [ ] Add the verified custom domain to Settings → Pages and then a `CNAME` file.
- [ ] Confirm GitHub's certificate and Enforce HTTPS.
- [ ] Replace canonical/social/sitemap URLs after domain migration.

## Operating model

- No Actions workflow is needed; GitHub Pages branch-source deployment is sufficient.
- The application CI schedule, quotas and containers must remain untouched.
- Web copy should update on real public application releases only; never publish private source URLs as public downloads.
