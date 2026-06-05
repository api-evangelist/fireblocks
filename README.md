# fireblocks (fireblocks)

Fireblocks is an institutional digital-asset and stablecoin infrastructure company providing MPC-secured custody, wallets (custodial and non-custodial / embedded), payments, tokenization, staking, smart contracts, off-exchange settlement, and DeFi security to trading firms, fintechs, exchanges, payment service providers, banks, financial institutions, and Web3 companies. The Fireblocks REST API exposes 236+ operations across 15 surface areas — Vaults, Transactions, Wallets, Assets, Exchange, Tokenization, Contracts, Staking, NFTs, Payments, Network/Off-Exchange, Compliance, Gas Station, Workspace Management, and Webhooks — alongside the separate Non-Custodial Wallet (NCW) API for embedded wallets.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Fireblocks Vaults API

Create and manage vault accounts, asset wallets, deposit addresses, attached tags, and balance inquiries. Vaults are the root container for MPC-secured keys, balances, and transactions inside a Fireblocks workspace. Supports paged listing, bulk address creation, customer-ref-id tagging, auto-fuel toggling, and UTXO/unspent-input enumeration.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Vaults
- Custody
- MPC

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-vaults-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-vaults-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-vaults-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/fireblocks-vault-account-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Transactions API

Create, cancel, drop, and query digital-asset transactions across all supported chains. Every transaction passes the workspace Policy Engine, is signed by the MPC quorum, and is broadcast under Fireblocks' fee-bump-and-rebroadcast logic. Supports transfers, raw signings, typed-message signings, contract calls, drop-and-replace, fee estimation, validate-address, and approval-request management.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Transactions
- MPC
- Custody

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-transactions-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-transactions-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-transactions-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/fireblocks-transaction-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Whitelisted Wallets API

Manage Fireblocks whitelisted destinations — internal wallets, external wallets, and whitelisted contracts. Internal wallets group addresses you own outside of vault accounts; external wallets identify counterparties (exchanges, payment processors, custodians). All approved destinations bypass one-time-address restrictions and accelerate the policy-engine quorum.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Wallets
- Whitelisting
- Compliance

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-wallets-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-wallets-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-wallets-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Blockchains and Assets API

Enumerate the blockchains and assets supported by the workspace — native coins, ERC-20s, SPL tokens, BRC-20s, NFTs — and register new asset/contract pairs. Returns asset metadata including contract address, native asset, decimals, and on-chain id used by the rest of the Fireblocks API.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Blockchains
- Assets

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-assets-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-assets-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-assets-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Exchange and Fiat Accounts API

Connect, read, and trade across exchange accounts and fiat (DDA) accounts. Manage exchange sub-accounts, perform internal exchange transfers, convert between assets, read manifests of trading pairs, fetch rates and balances, and surface Connected Accounts (Beta) and Trading (Beta) quotes/orders.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Exchanges
- Fiat
- Trading

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-exchange-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-exchange-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-exchange-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Tokenization API

Deploy, mint, burn, and manage tokens across the chains supported by Fireblocks Tokenization Engine. Covers ERC-20 fungible tokens, multichain stablecoins, asset tokenization, smart contract management, and the full token lifecycle. Pricing is 3-30 basis points on Assets Under Custody.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Tokenization
- Stablecoins
- Smart Contracts

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-tokenization-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-tokenization-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-tokenization-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Smart Contracts API

Deploy contract templates, manage deployed contracts, execute read/write contract interactions, and broker dApp connections via WalletConnect. Powers the Fireblocks DeFi security suite — every contract call passes the workspace Policy Engine and is simulated before MPC signing.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Smart Contracts
- dApps
- DeFi

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-contracts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-contracts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-contracts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Staking API

Execute and track staking operations across multiple proof-of-stake chains. Browse staking providers and validators, initiate stake / unstake / withdraw / claim-rewards actions, and query position state. Backs institutional Earn workflows for ETH, SOL, ADA, DOT, KSM, NEAR, TEZOS, MATIC, and more.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Staking
- DeFi

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-staking-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-staking-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-staking-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks NFTs API

Discover, index, and manage non-fungible tokens held in the workspace's vault accounts. List owned NFTs, fetch token-level metadata, refresh ownership state, and update token-spam classification.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- NFTs
- Tokens

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-nfts-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-nfts-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-nfts-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Payments API

Run institutional crypto payment flows — payment configs, payout instruction sets, and Smart Transfer tickets (atomic multi-leg asset transfers between two counterparties). Powers cross-border B2B settlement, OTC desks, PSP rails, and the Fireblocks Agentic Payments Suite.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Payments
- Stablecoins
- Payouts
- Smart Transfers

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-payments-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-payments-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-payments-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Network and Off-Exchange API

Configure Fireblocks Network connections (point-to-point connectivity layer between Fireblocks workspaces), set routing policies per asset, and operate Off-Exchange — Fireblocks' settlement layer that keeps collateral in MPC custody while mirroring balances to integrated exchanges.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Network
- Off-Exchange
- Settlement

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-network-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-network-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-network-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Compliance and Policy API

AML transaction screening, Travel Rule VASP messaging (FATF Recommendation 16), address registry lookups, and the workspace Policy Editor (Beta and V2). Wire third-party screening providers (Chainalysis, Elliptic, TRM) into the transaction lifecycle and codify the workspace's transaction-authorization rules.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Compliance
- AML
- Travel Rule
- Policy

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-compliance-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-compliance-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-compliance-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Gas Station API

Configure the Fireblocks Gas Station — auto-fuel logic that tops up native-asset balances in vault accounts so ERC-20 / SPL / contract-call transactions don't fail for lack of gas. Per-asset thresholds are workspace-configurable.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Gas Station
- Fees

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-gas-station-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-gas-station-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-gas-station-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Workspace Management API

Manage everything inside a Fireblocks workspace — API users, console users, user groups, audit logs, cosigners, signing keys, KeyLink external-key management, workspace freeze/unfreeze, and Admin Quorum administrative approvals.

- **Human URL:** [https://developers.fireblocks.com/reference/api-overview](https://developers.fireblocks.com/reference/api-overview)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Administrative
- Users
- Keys
- Audit

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [OpenAPI](openapi/fireblocks-workspace-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-workspace-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-workspace-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Fireblocks Webhooks API

Receive push notifications when workspace events occur — TRANSACTION_CREATED, TRANSACTION_STATUS_UPDATED, VAULT_ACCOUNT_ADDED, EMBEDDED_WALLET_DEVICE_PAIRED, SMART_TRANSFER events, and more. Each event is signed with RSA-SHA512 in the Fireblocks-Signature header so the consumer can verify authenticity before processing. Webhooks V2 surface adds destination management and replay-from-history.

- **Human URL:** [https://developers.fireblocks.com/reference/webhook-notifications](https://developers.fireblocks.com/reference/webhook-notifications)
- **Base URL:** `https://api.fireblocks.io/v1`

#### Tags

- Digital Assets
- Webhooks
- Events
- Push

#### Properties

- [Documentation](https://developers.fireblocks.com/reference/webhook-notifications)
- [OpenAPI](openapi/fireblocks-webhooks-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/fireblocks-webhooks-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/fireblocks-webhooks-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/fireblocks-webhook-event-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON-LD](json-ld/fireblocks-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

## Common Properties

- [Portal](https://www.fireblocks.com)
- [Documentation](https://developers.fireblocks.com)
- [Getting Started](https://developers.fireblocks.com/docs/quickstart)
- [Documentation](https://developers.fireblocks.com/reference/api-overview)
- [Pricing](https://www.fireblocks.com/pricing)
- [GitHub Organization](https://github.com/fireblocks)
- [OpenAPI](https://github.com/fireblocks/fireblocks-openapi-spec) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](https://github.com/fireblocks/fireblocks-ncw-open-api-spec) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Status Page](https://status.fireblocks.io)
- [About](https://www.fireblocks.com/about)
- [Contact Form](https://www.fireblocks.com/contact)
- [Careers](https://www.fireblocks.com/careers)
- [Terms of Service](https://www.fireblocks.com/legal/terms-of-service)
- [Privacy Policy](https://www.fireblocks.com/legal/privacy-notice)
- [Trust Center](https://trust.fireblocks.com/)
- [Blog](https://www.fireblocks.com/blog/)
- [News](https://www.fireblocks.com/newsroom/)
- [LinkedIn](https://www.linkedin.com/company/fireblocks/)
- [Twitter](https://x.com/fireblocks)
- [YouTube](https://www.youtube.com/c/Fireblocks)
- [Case Studies](https://www.fireblocks.com/customer-stories/)
- [Events](https://www.fireblocks.com/events/)
- [Training](https://academy.fireblocks.com/)
- [SDK](https://github.com/fireblocks/fireblocks-sdk-js)
- [SDK](https://github.com/fireblocks/ts-sdk)
- [SDK](https://github.com/fireblocks/fireblocks-sdk-py)
- [SDK](https://github.com/fireblocks/py-sdk)
- [SDK](https://github.com/fireblocks/java-sdk)
- [SDK](https://github.com/fireblocks/fireblocks-web3-provider)
- [SDK](https://github.com/fireblocks/hardhat-fireblocks)
- [SDK](https://github.com/fireblocks/fireblocks-defi-sdk)
- [SDK](https://github.com/fireblocks/fireblocks-defi-sdk-py)
- [SDK](https://github.com/fireblocks/fireblocks-json-rpc)
- [SDK](https://github.com/fireblocks/solana-web3-adapter)
- [SDK](https://github.com/fireblocks/fireblocks-xrp-sdk)
- [SDK](https://github.com/fireblocks/hbar-fireblocks-sdk)
- [SDK](https://github.com/fireblocks/cardano-raw-sdk)
- [SDK](https://github.com/fireblocks/move-fireblocks-sdk)
- [SDK](https://github.com/fireblocks/stacks-fireblocks-sdk)
- [SDK](https://github.com/fireblocks/seismic-sdk)
- [C L I](https://github.com/fireblocks/fireblocks-cli)
- [C L I](https://github.com/fireblocks/homebrew-fireblocks-cli)
- [Tool](https://github.com/fireblocks/recovery)
- [Tool](https://github.com/fireblocks/fireblocks-key-recovery-tool)
- [Tool](https://github.com/fireblocks/fireblocks-agent)
- [Tool](https://github.com/fireblocks/fireblocks-mcp)
- [Tool](https://github.com/fireblocks/x402-facilitator)
- [Tool](https://github.com/fireblocks/x402-agent)
- [Tool](https://github.com/fireblocks/mpc-lib)
- [Code Examples](https://github.com/fireblocks/developers-hub)
- [Code Examples](https://github.com/fireblocks/retail-demo)
- [Code Examples](https://github.com/fireblocks/tokenization-lab)
- [Code Examples](https://github.com/fireblocks/ncw-web-demo)
- [Code Examples](https://github.com/fireblocks/ncw-web-demo-v2)
- [Code Examples](https://github.com/fireblocks/ncw-backend-demo)
- [Code Examples](https://github.com/fireblocks/android-ncw-demo)
- [SDK](https://github.com/fireblocks/ncw-ios-sdk)
- [Code Examples](https://github.com/fireblocks/ncw-ios-demo)
- [SDK](https://github.com/fireblocks/react-native-ncw-sdk)
- [SDK](https://github.com/fireblocks/ew-ios-sdk)
- [Code Examples](https://github.com/fireblocks/ew-node-demo)
- [Code Examples](https://github.com/fireblocks/ew-backend-demo)
- [Code Examples](https://github.com/fireblocks/plugin-based-callback-handler)
- [Code Examples](https://github.com/fireblocks/btc_tx_validation)
- [Code Examples](https://github.com/fireblocks/eth_tx_validation)
- [Plans](https://plans/fireblocks-plans-pricing.yml)
- [Rate Limits](https://rate-limits/fireblocks-rate-limits.yml)
- [Fin Ops](https://finops/fireblocks-finops.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
