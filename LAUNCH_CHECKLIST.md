# Public launch checklist — Namerr website

Website repository: `Ragged-Labs/namerr-site` (kept separate from the private application repository and its Actions budget).

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

## Donations

- [ ] Choose a legitimate provider (e.g. GitHub Sponsors, Ko-fi or Buy Me a Coffee).
- [ ] Create and verify the recipient account / payment destination.
- [ ] Review fee, tax, legal and refund terms for the selected provider.
- [ ] Publish a clear voluntary contribution policy, with no false entitlement claim.
- [ ] Only then activate a direct public donation link.

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
