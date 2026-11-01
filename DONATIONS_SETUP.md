# Namerr donations — prelaunch activation checklist

**Status:** planned site copy only. The site is private; no payments are accepted.

## Buy Me a Coffee

- Proposed creator page: `buymeacoffee.com/namerr`.
- Account ownership, beneficiary and payout destination are **not verified**. Do not publish an actionable link to this proposed URL until confirmed.
- Confirm the payout currency, payment method, provider fees, taxation/accounting, refund terms and provider privacy policy.
- Once ownership is approved, link directly to the verified page with `rel="noopener noreferrer"` and label it as an external payment service.

## Bitcoin

- Proposed network is **Bitcoin mainnet (BTC)**, not an unrelated token, wrapped BTC or other blockchain network.
- The owner must provide and independently verify a **public receiving address** under their control. Never store or publish private keys, wallet seed/recovery phrases or signing credentials.
- Validate QR code bytes against the exact approved receiving address before publishing any image. Never use example or invented addresses for real transfers.
- Explain that transactions are often irreversible, amounts and addresses are recorded on a public blockchain, and network fees can apply.
- Lightning invoices would require a separate, explicit implementation and must not be mixed up with BTC mainnet addresses.

## Launch and privacy

- Supporting Namerr is strictly optional. A donation does not promise any feature, timeline, premium access or technical support.
- No account, wallet, QR code, payment button, checkout, cookies or third-party payment scripts are included in prelaunch pages.
- Update website Privacy and test outgoing links when enabling donations, then get explicit owner approval before publishing.
- Keep the website and new application repositories private until the deliberate public launch gate.

## Ownership

- Developer: **RaggedLabs Media**, brand domain `raggedlabs.media`, contact `contact@raggedlabs.media`.
- Website: `Ragged-Labs/namerr-site` (private).
- Reserved application home: `Ragged-Labs/namerr` (private placeholder).
- Existing application compatibility: `raggedred/emby_organiser_docker` (private).
