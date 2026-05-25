# Fireblocks (fireblocks)
Fireblocks is an institutional digital-asset and stablecoin infrastructure company providing MPC-secured custody, wallets (custodial and non-custodial / embedded), payments, tokenization, staking, smart contracts, off-exchange settlement, and DeFi security to trading firms, fintechs, exchanges, payment service providers, banks, financial institutions, and Web3 companies. The Fireblocks REST API exposes 236+ operations across 15 surface areas alongside the separate Non-Custodial Wallet (NCW) API for embedded wallets.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Digital Assets, Custody, MPC, Wallets, Tokenization, Stablecoins, Payments, Staking, DeFi, NFTs, Compliance, Travel Rule, Off-Exchange, Smart Contracts, Webhooks

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## API Surface

Base URL (production): `https://api.fireblocks.io/v1`
Base URL (sandbox):    `https://sandbox-api.fireblocks.io/v1`
Authentication:        JWT signed with RSA 4096 private key, `X-API-Key` header carries the workspace API user identifier, per-request body hash, 30-second expiry.

| Surface | Paths | Description |
|---|---|---|
| Vaults | 31 | Vault accounts, asset wallets, deposit addresses, balances, tags |
| Transactions | 18 | Transfers, raw signings, contract calls, drop-and-replace, approvals |
| Whitelisted Wallets | 12 | Internal wallets, external wallets, whitelisted contracts |
| Blockchains & Assets | 8 | Supported chains, asset registry, new-asset registration |
| Exchange & Fiat Accounts | 20 | Exchange/fiat/connected accounts, conversions, trading |
| Tokenization | 8 | Deploy/mint/burn fungible tokens and stablecoins |
| Smart Contracts | 17 | Templates, deployed contracts, interactions, dApp connections |
| Staking | 14 | Stake/unstake/withdraw across PoS chains |
| NFTs | 8 | Non-fungible token discovery and ownership |
| Payments | 23 | Payment flows, payouts, Smart Transfers (atomic multi-leg) |
| Network & Off-Exchange | 16 | Fireblocks Network connections, Off-Exchange settlement |
| Compliance & Policy | 21 | AML screening, Travel Rule, Policy Editor |
| Gas Station | 4 | Auto-fuel native-asset balances |
| Workspace Management | 25 | Users, keys, cosigners, audit logs, workspace freeze |
| Webhooks | 11 | Webhook destinations, signature verification, replay |

## APIs

### Fireblocks Vaults API
Create and manage vault accounts, asset wallets, deposit addresses, attached tags, and balance inquiries. Supports paged listing, bulk address creation, customer-ref-id tagging, auto-fuel toggling, and UTXO/unspent-input enumeration.

**Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-vaults-api-openapi.yml)
- [JSON Schema — Vault Account](json-schema/fireblocks-vault-account-schema.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld)
- [Naftiko Capability — Vaults](capabilities/vaults.yaml)

### Fireblocks Transactions API
Create, cancel, drop, and query digital-asset transactions across all supported chains. Every transaction passes the workspace Policy Engine, is signed by the MPC quorum, and is broadcast under Fireblocks' fee-bump-and-rebroadcast logic.

**Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)

- [OpenAPI](openapi/fireblocks-transactions-api-openapi.yml)
- [JSON Schema — Transaction](json-schema/fireblocks-transaction-schema.json)
- [Naftiko Capability — Transactions](capabilities/transactions.yaml)

### Fireblocks Whitelisted Wallets API
Manage internal wallets, external wallets, and whitelisted contracts. Approved destinations bypass one-time-address restrictions and accelerate the policy-engine quorum.

- [OpenAPI](openapi/fireblocks-wallets-api-openapi.yml)
- [Naftiko Capability — Wallets](capabilities/wallets.yaml)

### Fireblocks Blockchains and Assets API
Enumerate supported blockchains and assets and register new asset/contract pairs.

- [OpenAPI](openapi/fireblocks-assets-api-openapi.yml)
- [Naftiko Capability — Assets](capabilities/assets.yaml)

### Fireblocks Exchange and Fiat Accounts API
Connect, read, and trade across exchange accounts and fiat (DDA) accounts. Manage sub-accounts, internal transfers, conversions, manifests, rates, balances, and Connected Accounts (Beta).

- [OpenAPI](openapi/fireblocks-exchange-api-openapi.yml)
- [Naftiko Capability — Exchange](capabilities/exchange.yaml)

### Fireblocks Tokenization API
Deploy, mint, burn, and manage fungible tokens and stablecoins across supported chains via the Fireblocks Tokenization Engine.

- [OpenAPI](openapi/fireblocks-tokenization-api-openapi.yml)
- [Naftiko Capability — Tokenization](capabilities/tokenization.yaml)

### Fireblocks Smart Contracts API
Contract templates, deployed contracts, read/write interactions, and WalletConnect-mediated dApp connections — all protected by the Policy Engine and transaction simulation.

- [OpenAPI](openapi/fireblocks-contracts-api-openapi.yml)
- [Naftiko Capability — Contracts](capabilities/contracts.yaml)

### Fireblocks Staking API
Execute and track staking operations across multiple proof-of-stake chains (ETH, SOL, ADA, DOT, KSM, NEAR, TEZOS, MATIC, and more).

- [OpenAPI](openapi/fireblocks-staking-api-openapi.yml)
- [Naftiko Capability — Staking](capabilities/staking.yaml)

### Fireblocks NFTs API
Discover, index, and manage non-fungible tokens held in workspace vault accounts.

- [OpenAPI](openapi/fireblocks-nfts-api-openapi.yml)
- [Naftiko Capability — NFTs](capabilities/nfts.yaml)

### Fireblocks Payments API
Run institutional crypto payment flows — payment configs, payout instruction sets, and Smart Transfer tickets (atomic multi-leg asset settlement between two counterparties).

- [OpenAPI](openapi/fireblocks-payments-api-openapi.yml)
- [Naftiko Capability — Payments](capabilities/payments.yaml)

### Fireblocks Network and Off-Exchange API
Fireblocks Network point-to-point connectivity and Off-Exchange — keep collateral in MPC custody while mirroring balances to integrated exchanges.

- [OpenAPI](openapi/fireblocks-network-api-openapi.yml)
- [Naftiko Capability — Network](capabilities/network.yaml)

### Fireblocks Compliance and Policy API
AML transaction screening, Travel Rule (FATF R.16) VASP messaging, address registry, and the workspace Policy Editor (Beta and V2).

- [OpenAPI](openapi/fireblocks-compliance-api-openapi.yml)
- [Naftiko Capability — Compliance](capabilities/compliance.yaml)

### Fireblocks Gas Station API
Configure auto-fuel logic that tops up native-asset balances in vault accounts so contract calls don't fail for lack of gas.

- [OpenAPI](openapi/fireblocks-gas-station-api-openapi.yml)
- [Naftiko Capability — Gas Station](capabilities/gas-station.yaml)

### Fireblocks Workspace Management API
API users, console users, user groups, audit logs, cosigners, signing keys, KeyLink external-key management, workspace freeze, and Admin Quorum.

- [OpenAPI](openapi/fireblocks-workspace-api-openapi.yml)
- [Naftiko Capability — Workspace](capabilities/workspace.yaml)

### Fireblocks Webhooks API
Receive push notifications for workspace events. Every event is signed RSA-SHA512 in the `Fireblocks-Signature` header.

**Human URL:** [https://developers.fireblocks.com/reference/webhook-notifications](https://developers.fireblocks.com/reference/webhook-notifications)

- [OpenAPI](openapi/fireblocks-webhooks-api-openapi.yml)
- [JSON Schema — Webhook Event](json-schema/fireblocks-webhook-event-schema.json)
- [Naftiko Capability — Webhooks](capabilities/webhooks.yaml)

## Common Properties

- [Portal — fireblocks.com](https://www.fireblocks.com)
- [Documentation — developers.fireblocks.com](https://developers.fireblocks.com)
- [GettingStarted](https://developers.fireblocks.com/docs/quickstart)
- [Pricing](https://www.fireblocks.com/pricing)
- [GitHubOrganization](https://github.com/fireblocks)
- [StatusPage](https://status.fireblocks.io)
- [TrustCenter](https://trust.fireblocks.com/)
- [TermsOfService](https://www.fireblocks.com/legal/terms-of-service)
- [PrivacyPolicy](https://www.fireblocks.com/legal/privacy-notice)
- [Blog](https://www.fireblocks.com/blog/)
- [Training — Fireblocks Academy](https://academy.fireblocks.com/)
- [SDK — TypeScript / JavaScript](https://github.com/fireblocks/fireblocks-sdk-js)
- [SDK — TypeScript next-gen](https://github.com/fireblocks/ts-sdk)
- [SDK — Python](https://github.com/fireblocks/fireblocks-sdk-py)
- [SDK — Python next-gen](https://github.com/fireblocks/py-sdk)
- [SDK — Java](https://github.com/fireblocks/java-sdk)
- [SDK — EIP-1193 Web3 Provider](https://github.com/fireblocks/fireblocks-web3-provider)
- [SDK — Hardhat plugin](https://github.com/fireblocks/hardhat-fireblocks)
- [SDK — DeFi (TypeScript)](https://github.com/fireblocks/fireblocks-defi-sdk)
- [SDK — DeFi (Python)](https://github.com/fireblocks/fireblocks-defi-sdk-py)
- [SDK — Solana adapter](https://github.com/fireblocks/solana-web3-adapter)
- [SDK — XRPL](https://github.com/fireblocks/fireblocks-xrp-sdk)
- [SDK — Hedera](https://github.com/fireblocks/hbar-fireblocks-sdk)
- [SDK — Cardano RAW](https://github.com/fireblocks/cardano-raw-sdk)
- [SDK — Movement](https://github.com/fireblocks/move-fireblocks-sdk)
- [SDK — Stacks](https://github.com/fireblocks/stacks-fireblocks-sdk)
- [SDK — Seismic](https://github.com/fireblocks/seismic-sdk)
- [SDK — NCW iOS](https://github.com/fireblocks/ncw-ios-sdk)
- [SDK — React Native NCW](https://github.com/fireblocks/react-native-ncw-sdk)
- [SDK — Embedded Wallets iOS](https://github.com/fireblocks/ew-ios-sdk)
- [CLI — Fireblocks CLI](https://github.com/fireblocks/fireblocks-cli)
- [CLI — Homebrew tap](https://github.com/fireblocks/homebrew-fireblocks-cli)
- [Tool — Recovery Utility](https://github.com/fireblocks/recovery)
- [Tool — Key Recovery Tool](https://github.com/fireblocks/fireblocks-key-recovery-tool)
- [Tool — Fireblocks Agent (on-prem external keys)](https://github.com/fireblocks/fireblocks-agent)
- [Tool — Fireblocks MCP Server](https://github.com/fireblocks/fireblocks-mcp)
- [Tool — x402 Payment Facilitator](https://github.com/fireblocks/x402-facilitator)
- [Tool — x402 Payment Agent](https://github.com/fireblocks/x402-agent)
- [Tool — MPC Cryptography Library](https://github.com/fireblocks/mpc-lib)
- [CodeExamples — Developers Hub](https://github.com/fireblocks/developers-hub)
- [CodeExamples — Retail Demo](https://github.com/fireblocks/retail-demo)
- [CodeExamples — Tokenization Lab](https://github.com/fireblocks/tokenization-lab)
- [CodeExamples — NCW Web Demo](https://github.com/fireblocks/ncw-web-demo)
- [CodeExamples — Plugin-based Callback Handler](https://github.com/fireblocks/plugin-based-callback-handler)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Fireblocks Vaults API](openapi/fireblocks-vaults-api-openapi.yml)
- [Fireblocks Transactions API](openapi/fireblocks-transactions-api-openapi.yml)
- [Fireblocks Whitelisted Wallets API](openapi/fireblocks-wallets-api-openapi.yml)
- [Fireblocks Blockchains and Assets API](openapi/fireblocks-assets-api-openapi.yml)
- [Fireblocks Exchange and Fiat Accounts API](openapi/fireblocks-exchange-api-openapi.yml)
- [Fireblocks Tokenization API](openapi/fireblocks-tokenization-api-openapi.yml)
- [Fireblocks Smart Contracts API](openapi/fireblocks-contracts-api-openapi.yml)
- [Fireblocks Staking API](openapi/fireblocks-staking-api-openapi.yml)
- [Fireblocks NFTs API](openapi/fireblocks-nfts-api-openapi.yml)
- [Fireblocks Payments API](openapi/fireblocks-payments-api-openapi.yml)
- [Fireblocks Network and Off-Exchange API](openapi/fireblocks-network-api-openapi.yml)
- [Fireblocks Compliance and Policy API](openapi/fireblocks-compliance-api-openapi.yml)
- [Fireblocks Gas Station API](openapi/fireblocks-gas-station-api-openapi.yml)
- [Fireblocks Workspace Management API](openapi/fireblocks-workspace-api-openapi.yml)
- [Fireblocks Webhooks API](openapi/fireblocks-webhooks-api-openapi.yml)

### JSON Schema

- [Vault Account](json-schema/fireblocks-vault-account-schema.json)
- [Transaction](json-schema/fireblocks-transaction-schema.json)
- [Webhook Event](json-schema/fireblocks-webhook-event-schema.json)

### JSON-LD

- [Fireblocks Context](json-ld/fireblocks-context.jsonld)

### Capabilities (Naftiko)

- [Vaults](capabilities/vaults.yaml)
- [Transactions](capabilities/transactions.yaml)
- [Wallets](capabilities/wallets.yaml)
- [Assets](capabilities/assets.yaml)
- [Exchange](capabilities/exchange.yaml)
- [Tokenization](capabilities/tokenization.yaml)
- [Contracts](capabilities/contracts.yaml)
- [Staking](capabilities/staking.yaml)
- [NFTs](capabilities/nfts.yaml)
- [Payments](capabilities/payments.yaml)
- [Network](capabilities/network.yaml)
- [Compliance](capabilities/compliance.yaml)
- [Gas Station](capabilities/gas-station.yaml)
- [Workspace](capabilities/workspace.yaml)
- [Webhooks](capabilities/webhooks.yaml)

### Commercial artifacts

- [Plans / Pricing](plans/fireblocks-plans-pricing.yml)
- [Rate Limits](rate-limits/fireblocks-rate-limits.yml)
- [FinOps Definition](finops/fireblocks-finops.yml)

## Maintainers

**FN:** Kin Lane

**Email:** info@apievangelist.com
