# Fireblocks

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

Fireblocks is an institutional digital-asset and stablecoin infrastructure company providing MPC-secured custody, wallets (custodial and non-custodial / embedded), payments, tokenization, staking, smart contracts, off-exchange settlement, and DeFi security to trading firms, fintechs, exchanges, payment service providers, banks, financial institutions, and Web3 companies. The Fireblocks REST API exposes 236+ operations across 15 surface areas — Vaults, Transactions, Wallets, Assets, Exchange, Tokenization, Contracts, Staking, NFTs, Payments, Network/Off-Exchange, Compliance, Gas Station, Workspace Management, and Webhooks — alongside the separate Non-Custodial Wallet (NCW) API for embedded wallets.

**Areas:** Digital Assets · Custody · Vault · Transaction · Tokenization · Stablecoins

## Fireblocks on APIs.io

Everything profiled for Fireblocks is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/fireblocks/](https://apis.io/providers/fireblocks/)** — or go straight to one of the APIs or properties below.

### APIs (35)

- [Fireblocks Vaults API](https://apis.io/apis/fireblocks/fireblocks-vaults-api/) — Create and manage vault accounts, asset wallets, deposit addresses, attached tags, and balance inquiries. Vaults are the root container for MPC-secured…
- [Fireblocks Transactions API](https://apis.io/apis/fireblocks/fireblocks-transactions-api/) — Create, cancel, drop, and query digital-asset transactions across all supported chains. Every transaction passes the workspace Policy Engine, is signed by…
- [Fireblocks Tokenization API](https://apis.io/apis/fireblocks/fireblocks-tokenization-api/) — Deploy, mint, burn, and manage tokens across the chains supported by Fireblocks Tokenization Engine. Covers ERC-20 fungible tokens, multichain stablecoins,…
- [Fireblocks Staking API](https://apis.io/apis/fireblocks/fireblocks-staking-api/) — Execute and track staking operations across multiple proof-of-stake chains. Browse staking providers and validators, initiate stake / unstake / withdraw /…
- [Fireblocks NFTs API](https://apis.io/apis/fireblocks/fireblocks-nfts-api/) — Discover, index, and manage non-fungible tokens held in the workspace's vault accounts. List owned NFTs, fetch token-level metadata, refresh ownership…
- [Fireblocks Compliance and Policy API](https://apis.io/apis/fireblocks/fireblocks-compliance-api/) — AML transaction screening, Travel Rule VASP messaging (FATF Recommendation 16), address registry lookups, and the workspace Policy Editor (Beta and V2).…
- [Fireblocks Gas Station API](https://apis.io/apis/fireblocks/fireblocks-gas-station-api/) — Configure the Fireblocks Gas Station — auto-fuel logic that tops up native-asset balances in vault accounts so ERC-20 / SPL / contract-call transactions…
- [Fireblocks Webhooks API](https://apis.io/apis/fireblocks/fireblocks-webhooks-api/) — Receive push notifications when workspace events occur — TRANSACTION_CREATED, TRANSACTION_STATUS_UPDATED, VAULT_ACCOUNT_ADDED,…
- [fireblocks Approval Requests API](https://apis.io/apis/fireblocks/fireblocks-approval-requests-api/) — The Approval Requests API from fireblocks — 2 operation(s) for approval requests.
- [fireblocks Blockchains & Assets API](https://apis.io/apis/fireblocks/fireblocks-blockchains-assets-api/) — The Blockchains & Assets API from fireblocks — 8 operation(s) for blockchains & assets.
- [fireblocks Connected Accounts (Beta) API](https://apis.io/apis/fireblocks/fireblocks-connected-accounts-beta-api/) — The Connected Accounts (Beta) API from fireblocks — 5 operation(s) for connected accounts (beta).
- [fireblocks Contract Interactions API](https://apis.io/apis/fireblocks/fireblocks-contract-interactions-api/) — The Contract Interactions API from fireblocks — 4 operation(s) for contract interactions.
- [fireblocks Contract Templates API](https://apis.io/apis/fireblocks/fireblocks-contract-templates-api/) — The Contract Templates API from fireblocks — 5 operation(s) for contract templates.
- [fireblocks Cosigners (Beta) API](https://apis.io/apis/fireblocks/fireblocks-cosigners-beta-api/) — The Cosigners (Beta) API from fireblocks — 5 operation(s) for cosigners (beta).
- [fireblocks dApp Connections API](https://apis.io/apis/fireblocks/fireblocks-dapp-connections-api/) — The dApp Connections API from fireblocks — 3 operation(s) for dapp connections.
- [fireblocks Deployed Contracts API](https://apis.io/apis/fireblocks/fireblocks-deployed-contracts-api/) — The Deployed Contracts API from fireblocks — 5 operation(s) for deployed contracts.
- [fireblocks Exchange Accounts API](https://apis.io/apis/fireblocks/fireblocks-exchange-accounts-api/) — The Exchange Accounts API from fireblocks — 7 operation(s) for exchange accounts.
- [fireblocks Fiat Accounts API](https://apis.io/apis/fireblocks/fireblocks-fiat-accounts-api/) — The Fiat Accounts API from fireblocks — 4 operation(s) for fiat accounts.
- [fireblocks Network API](https://apis.io/apis/fireblocks/fireblocks-fireblocks-network-api/) — The Fireblocks Network API from fireblocks — 11 operation(s) for fireblocks network.
- [fireblocks Job Management API](https://apis.io/apis/fireblocks/fireblocks-job-management-api/) — The Job Management API from fireblocks — 6 operation(s) for job management.
- [fireblocks Key Link API](https://apis.io/apis/fireblocks/fireblocks-key-link-api/) — The Key Link API from fireblocks — 5 operation(s) for key link.
- [fireblocks Keys (Beta) API](https://apis.io/apis/fireblocks/fireblocks-keys-beta-api/) — The Keys (Beta) API from fireblocks — 2 operation(s) for keys (beta).
- [fireblocks Off Exchange API](https://apis.io/apis/fireblocks/fireblocks-off-exchange-api/) — The Off Exchange API from fireblocks — 5 operation(s) for off exchange.
- [fireblocks Payments - Flows API](https://apis.io/apis/fireblocks/fireblocks-payments-flows-api/) — The Payments - Flows API from fireblocks — 5 operation(s) for payments - flows.
- [fireblocks Payments - Payout API](https://apis.io/apis/fireblocks/fireblocks-payments-payout-api/) — The Payments - Payout API from fireblocks — 3 operation(s) for payments - payout.
- [fireblocks Policy Editor (Beta) API](https://apis.io/apis/fireblocks/fireblocks-policy-editor-beta-api/) — The Policy Editor (Beta) API from fireblocks — 3 operation(s) for policy editor (beta).
- [fireblocks Policy Editor V2 (Beta) API](https://apis.io/apis/fireblocks/fireblocks-policy-editor-v2-beta-api/) — The Policy Editor V2 (Beta) API from fireblocks — 2 operation(s) for policy editor v2 (beta).
- [fireblocks Smart Transfers API](https://apis.io/apis/fireblocks/fireblocks-smart-transfers-api/) — The Smart Transfers API from fireblocks — 15 operation(s) for smart transfers.
- [fireblocks Tags API](https://apis.io/apis/fireblocks/fireblocks-tags-api/) — The Tags API from fireblocks — 2 operation(s) for tags.
- [fireblocks Trading (Beta) API](https://apis.io/apis/fireblocks/fireblocks-trading-beta-api/) — The Trading (Beta) API from fireblocks — 4 operation(s) for trading (beta).
- [fireblocks Webhooks V2 API](https://apis.io/apis/fireblocks/fireblocks-webhooks-v2-api/) — The Webhooks V2 API from fireblocks — 9 operation(s) for webhooks v2.
- [fireblocks Whitelisted Contracts API](https://apis.io/apis/fireblocks/fireblocks-whitelisted-contracts-api/) — The Whitelisted Contracts API from fireblocks — 3 operation(s) for whitelisted contracts.
- [fireblocks Whitelisted External Wallets API](https://apis.io/apis/fireblocks/fireblocks-whitelisted-external-wallets-api/) — The Whitelisted External Wallets API from fireblocks — 4 operation(s) for whitelisted external wallets.
- [fireblocks Whitelisted Internal Wallets API](https://apis.io/apis/fireblocks/fireblocks-whitelisted-internal-wallets-api/) — The Whitelisted Internal Wallets API from fireblocks — 5 operation(s) for whitelisted internal wallets.
- [fireblocks Workspace Management API](https://apis.io/apis/fireblocks/fireblocks-workspace-management-api/) — The Workspace Management API from fireblocks — 13 operation(s) for workspace management.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Fireblocks Agentic Access](https://apis.io/agentic-access/fireblocks/fireblocks-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Fireblocks Transaction](https://apis.io/schemas/fireblocks/fireblocks-transaction/)
- [Fireblocks Vault Account](https://apis.io/schemas/fireblocks/fireblocks-vault-account/)
- [Fireblocks Webhook Event](https://apis.io/schemas/fireblocks/fireblocks-webhook-event/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Fireblocks Context](https://apis.io/jsonld/fireblocks/fireblocks-context/)

#### Collections (77)

Postman and Open Collection request collections.

- [Fireblocks Blockchains and Assets Approval Requests API](https://apis.io/collections/fireblocks/open-fireblocks-approval-requests-api/)
- [Fireblocks Blockchains and Assets API](https://apis.io/collections/fireblocks/open-fireblocks-assets-api/)
- [Fireblocks Blockchains and Assets Approval Requests Blockchains & Assets API](https://apis.io/collections/fireblocks/open-fireblocks-blockchains-assets-api/)
- [Fireblocks Blockchains and Assets Approval Requests Compliance API](https://apis.io/collections/fireblocks/open-fireblocks-compliance-api/)
- [Fireblocks Blockchains and Assets Approval Requests Connected Accounts (Beta) API](https://apis.io/collections/fireblocks/open-fireblocks-connected-accounts-beta-api/)
- [Fireblocks Blockchains and Assets Approval Requests Contract Interactions API](https://apis.io/collections/fireblocks/open-fireblocks-contract-interactions-api/)
- [Fireblocks Blockchains and Assets Approval Requests Contract Templates API](https://apis.io/collections/fireblocks/open-fireblocks-contract-templates-api/)
- [Fireblocks Smart Contracts API](https://apis.io/collections/fireblocks/open-fireblocks-contracts-api/)
- [Fireblocks Blockchains and Assets Approval Requests Cosigners (Beta) API](https://apis.io/collections/fireblocks/open-fireblocks-cosigners-beta-api/)
- [Fireblocks Blockchains and Assets Approval Requests dApp Connections API](https://apis.io/collections/fireblocks/open-fireblocks-dapp-connections-api/)
- [Fireblocks Blockchains and Assets Approval Requests Deployed Contracts API](https://apis.io/collections/fireblocks/open-fireblocks-deployed-contracts-api/)
- [Fireblocks Blockchains and Assets Approval Requests Exchange Accounts API](https://apis.io/collections/fireblocks/open-fireblocks-exchange-accounts-api/)
- [Fireblocks Exchange and Fiat Accounts API](https://apis.io/collections/fireblocks/open-fireblocks-exchange-api/)
- [Fireblocks Blockchains and Assets Approval Requests Fiat Accounts API](https://apis.io/collections/fireblocks/open-fireblocks-fiat-accounts-api/)
- [Fireblocks Blockchains and Assets Approval Requests Fireblocks Network API](https://apis.io/collections/fireblocks/open-fireblocks-fireblocks-network-api/)
- [Fireblocks Blockchains and Assets Approval Requests Gas Station API](https://apis.io/collections/fireblocks/open-fireblocks-gas-station-api/)
- [Fireblocks Blockchains and Assets Approval Requests Job Management API](https://apis.io/collections/fireblocks/open-fireblocks-job-management-api/)
- [Fireblocks Blockchains and Assets Approval Requests Key Link API](https://apis.io/collections/fireblocks/open-fireblocks-key-link-api/)
- [Fireblocks Blockchains and Assets Approval Requests Keys (Beta) API](https://apis.io/collections/fireblocks/open-fireblocks-keys-beta-api/)
- [Fireblocks Network and Off-Exchange API](https://apis.io/collections/fireblocks/open-fireblocks-network-api/)
- [Fireblocks Blockchains and Assets Approval Requests NFTs API](https://apis.io/collections/fireblocks/open-fireblocks-nfts-api/)
- [Fireblocks Blockchains and Assets Approval Requests Off Exchange API](https://apis.io/collections/fireblocks/open-fireblocks-off-exchange-api/)
- [Fireblocks Payments API](https://apis.io/collections/fireblocks/open-fireblocks-payments-api/)
- [Fireblocks Blockchains and Assets Approval Requests Payments - Flows API](https://apis.io/collections/fireblocks/open-fireblocks-payments-flows-api/)
- [Fireblocks Blockchains and Assets Approval Requests Payments - Payout API](https://apis.io/collections/fireblocks/open-fireblocks-payments-payout-api/)
- …and 52 more published on APIs.io

#### Governance rules (2)

Spectral rulesets for the provider's contracts.

- [Fireblocks — fireblocks network link rules](https://apis.io/rules/fireblocks/fireblocks-fireblocks-network-link-spectral-rules/)
- [Fireblocks — jsonschema rules](https://apis.io/rules/fireblocks/fireblocks-jsonschema-spectral-rules/)

#### Security (3)

Authentication, trust centre, and vulnerability disclosure.

- [Fireblocks Authentication](https://apis.io/security/fireblocks/fireblocks-authentication/)
- [Fireblocks Domain Security](https://apis.io/security/fireblocks/fireblocks-domain-security/)
- [Fireblocks Trust Center](https://apis.io/security/fireblocks/fireblocks-trust-center/)

#### Plans and pricing (2)

Published plans, tiers and prices.

- [Fireblocks Plans Pricing](https://apis.io/plans/fireblocks/fireblocks-plans-pricing/)
- [Fireblocks Price Estimates](https://apis.io/plans/fireblocks/fireblocks-price-estimates/)

#### Rate limits (1)

Published request limits.

- [Fireblocks Rate Limits](https://apis.io/rate-limits/fireblocks/fireblocks-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Fireblocks Finops](https://apis.io/finops/fireblocks/fireblocks-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.fireblocks.com/)
- [Documentation](https://developers.fireblocks.com)
- [Getting started](https://developers.fireblocks.com/docs/quickstart)
- [Pricing](https://www.fireblocks.com/pricing)
- [Changelog](https://developers.fireblocks.com/changelog)
- [Blog](https://www.fireblocks.com/blog/)
- [Trust centre](https://trust.fireblocks.com/)
- [Terms of service](https://www.fireblocks.com/legal/terms-of-service)
- [Privacy policy](https://www.fireblocks.com/legal/privacy-notice)
- [GitHub](https://github.com/fireblocks)
- [Status](https://status.fireblocks.io)

## API Evangelist rating

**Kin Score 67.2** — exemplar · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 75.0 |
| Contract quality | 61.8 |
| Contract governance | 54.5 |
| Operational transparency | 44.7 |
| Developer ergonomics | 70.2 |
| Access clarity | 68.4 |

**Agent readiness 38.0** — agent-ready

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | documented (partial credit) |
| MCP Server | — |
| Auth Clarity | bearer (partial credit) |
| Idempotency | verified |
| Error Semantics | verified |
| OpenAPI Examples | partial |
| Rate Limit Signal | documented (partial credit) |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |
| Pagination Ratio | partial |
| Operation Distinctiveness | distinct |

**Regulatory alignment 29.4** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/fireblocks/](https://apis.io/providers/fireblocks/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Fireblocks: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/fireblocks/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
