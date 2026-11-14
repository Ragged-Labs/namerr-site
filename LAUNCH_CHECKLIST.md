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
- [x] No public app download or paid subscription is active; voluntary Buy Me a Coffee support is linked. Bitcoin is not yet available.
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
- [x] Owner-provided Buy Me a Coffee link and matching QR code are present.
- [ ] Verify any additional donation destinations and obtain owner approval before activation.

## Product community launch

- [ ] Decide when to make `Ragged-Labs/namerr` public.
- [ ] Maintain or migrate historic Docker image/update identifiers without breaking existing installations.
- [ ] Reuse full website drafts from `archive/website-v1-before-coming-soon` and the private feature work without overwriting Coming Soon prematurely.
- [ ] Announce official release only after public access and downloads are verified.

## Cross-platform distribution launch requirements (DIST-01)

- [x] Public prelaunch site differentiates Docker/Unraid, Windows and macOS as development targets and links a platform selector, with no active install/download buttons.
- [x] Website explicitly marks Unraid drive placement as host-specific, not a Windows/macOS desktop capability.
- [ ] Validate Windows 11 x64 installer signing, internal/external/SMB storage permissions, safe writes and recovery.
- [ ] Validate Apple-silicon macOS signed/notarised DMG, permissions and internal/external/SMB storage. Decide Intel support after testing.
- [ ] Verify rollback/Undo/interruption safeguards per storage type; default unvalidated paths to scan/preview only.
- [ ] Validate separate platform release repositories and public GitHub Release artefacts before linking downloads.
- [ ] Publish screenshot-based installer, permissions, upgrade and recovery user guides per platform before public launch.
