# Namerr public-launch checklist

The public website intentionally shows **Coming Soon**. Do not replace it with installation, donation or community features until these checks pass.

## Application and installer

- [ ] Confirm the official public application repository, licence and publishing rights.
- [ ] Validate public Unraid, Docker and planned desktop packages as appropriate.
- [ ] Verify installation, appdata compatibility, permissions, media safety, rollback and upgrade instructions.
- [ ] Document supported versions, known issues, public issue reporting and support expectations.
- [ ] Do not link private repositories, inactive packages or unverified Docker images as if available to the public.

## Website

- [x] Branded Coming Soon homepage with Namerr's original N artwork.
- [x] Public contact email and RaggedLabs Media identity.
- [x] Active development and planned feature descriptions clearly distinguished.
- [x] No public download, paid subscription or donation action is active.
- [ ] Confirm GitHub Pages renders on mobile and desktop and verify all visible links.
- [ ] Complete the future full-site copy and user help before replacing Coming Soon.
- [ ] Review website security and privacy disclosures before enabling any integrations.

## Repository protection

- [ ] Activate the `main` branch ruleset under Settings → Rules → Rulesets.
- [ ] Confirm PR required, branch deletion blocked, force pushes blocked and linear history enabled.
- [ ] Confirm ruleset appears in GitHub's repository rulesets list. See [REPOSITORY_PROTECTION.md](REPOSITORY_PROTECTION.md).
- [ ] Add dependable website checks before requiring any check names in the ruleset.
- [ ] Re-evaluate review approvals when more maintainers join.

## Donation options (future)

- [ ] Verify control of the proposed Buy Me a Coffee `/namerr` recipient page and payout account.
- [ ] Verify a dedicated public BTC mainnet receiving address; never expose recovery phrases/private keys.
- [ ] Independently test any wallet QR image against the wallet address and network.
- [ ] Disclose relevant provider fees, privacy, tax, irreversible transfers and optional support nature.
- [ ] Seek owner's explicit approval before making donation links active.

## Product community launch

- [ ] Decide when to make `Ragged-Labs/namerr` public.
- [ ] Maintain or migrate historic Docker image/update identifiers without breaking existing installations.
- [ ] Reuse full website drafts from `archive/website-v1-before-coming-soon` and the private feature work without overwriting Coming Soon prematurely.
- [ ] Announce official release only after public access and downloads are verified.
