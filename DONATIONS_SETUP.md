# Namerr donations — prelaunch activation checklist

**Status:** the private website draft links to the owner-confirmed Buy Me a Coffee creator page. No payments are processed by the website itself. Bitcoin remains inactive. Publication of the website is still on hold.

## Buy Me a Coffee

- **Owner-confirmed creator page:** `https://www.buymeacoffee.com/namerr` (confirmed 1 November 2026).
- The website draft uses a clearly labelled external link with `target="_blank"` and `rel="noopener noreferrer"`; it does not embed checkout scripts or collect payment information.
- Account/page identity has been confirmed by the project owner. The payout destination and platform checkout were **not independently tested** by the assistant.
- Before public promotion, review payment fees, payout currency, account eligibility, taxation/accounting, refund terms and Buy Me a Coffee privacy terms. Confirm checkout with the actual creator account rather than relying solely on the public username.

## Bitcoin

- Proposed network is **Bitcoin mainnet (BTC)**, not an unrelated token, wrapped BTC or other blockchain network.
- The owner must provide and independently verify a **public receiving address** under their control. Never store or publish private keys, wallet seed/recovery phrases or signing credentials.
- Validate QR code bytes against the exact approved receiving address before publishing any image. Never use example or invented addresses for real transfers.
- Explain that transactions are often irreversible, amounts and addresses are recorded on a public blockchain, and network fees can apply.
- Lightning invoices would require a separate, explicit implementation and must not be mixed up with BTC mainnet addresses.

## Launch and privacy

- Supporting Namerr is strictly optional. A donation does not promise any feature, timeline, premium access or technical support.
- The draft contains a direct, owner-confirmed external Buy Me a Coffee link; no website-hosted checkout, cookies, payment scripts, Bitcoin wallet address or QR code is included.
- Update website Privacy and test outgoing links when enabling donations, then get explicit owner approval before publishing.
- Keep the website and new application repositories private until the deliberate public launch gate.

## Ownership

- Developer: **RaggedLabs Media**, brand domain `raggedlabs.media`, contact `contact@raggedlabs.media`.
- Website: `Ragged-Labs/namerr-site` (private).
- Reserved application home: `Ragged-Labs/namerr` (private placeholder).
- Existing application compatibility: `raggedred/emby_organiser_docker` (private).
