# Ankr

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

Ankr is a Web3 infrastructure provider whose multichain RPC, Advanced API, liquid staking,
contract automation, and Rollup-as-a-Service products serve developers, exchanges, and
enterprises across 80+ blockchains. The Node API exposes JSON-RPC and WebSocket endpoints at
rpc.ankr.com/{chain}; the Advanced API (AAPI) layers an indexed query surface across 19 EVM
mainnets for NFT, token, and historical-data reads. Ankr also operates liquid staking pools
(ankrETH, ankrBNB, ankrPOL, ankrAVAX, ankrFTM, ankrDOT, ankrFLOW), a contract automation
service on BNB Smart Chain, and an enterprise Rollup-as-a-Service practice that supports OP
Stack, Polygon CDK, and Arbitrum Orbit variants. Infrastructure runs as a global DePIN of
bare-metal nodes in 30+ regions serving roughly 8 billion daily RPC requests.

**Areas:** Web3 · EVM · NFT · Real-Time · Ethereum

## Ankr on APIs.io

Everything profiled for Ankr is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/ankr/](https://apis.io/providers/ankr/)** — or go straight to one of the APIs or properties below.

### APIs (8)

- [AnkrScan Block Explorer](https://apis.io/apis/ankr/ankr-block-explorer/) — AnkrScan is Ankr's multi-chain block explorer covering EVM and non-EVM networks. It is a hosted UI consuming Ankr's Node API and Advanced API and does not…
- [ankr Metrics API](https://apis.io/apis/ankr/ankr-metrics-api/) — Liquid staking pool statistics (TVL, APR, holders, supply).
- [ankr NFT API](https://apis.io/apis/ankr/ankr-nft-api/) — NFT methods — ownership, metadata, holders, and transfer history.
- [ankr Query API](https://apis.io/apis/ankr/ankr-query-api/) — Query methods — blockchain statistics, blocks, logs, transactions, interactions.
- [ankr Ratio API](https://apis.io/apis/ankr/ankr-ratio-api/) — Trustless exchange ratio between native and liquid staking tokens.
- [ankr Tasks API](https://apis.io/apis/ankr/ankr-tasks-api/) — Time-based and event-triggered automation tasks.
- [ankr Token API](https://apis.io/apis/ankr/ankr-token-api/) — Token methods — balances, prices, holders, currencies, and transfers.
- [ankr Validators API](https://apis.io/apis/ankr/ankr-validators-api/) — Validator metadata, unbond times, reward release windows.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Arazzo workflows (9)

Multi-step workflows that chain operations into a business task.

- [Ankr Block And Log Inspection](https://apis.io/arazzos/ankr/ankr-block-log-inspection-workflow/)
- [Ankr Chain Overview](https://apis.io/arazzos/ankr/ankr-chain-overview-workflow/)
- [Ankr NFT Collection Audit](https://apis.io/arazzos/ankr/ankr-nft-collection-audit-workflow/)
- [Ankr Wallet NFT Inventory](https://apis.io/arazzos/ankr/ankr-nft-inventory-workflow/)
- [Ankr Token Holder Distribution](https://apis.io/arazzos/ankr/ankr-token-holder-distribution-workflow/)
- [Ankr Token Price And History](https://apis.io/arazzos/ankr/ankr-token-price-and-history-workflow/)
- [Ankr Transaction Deep Dive](https://apis.io/arazzos/ankr/ankr-transaction-deep-dive-workflow/)
- [Ankr Wallet Cross-Chain Activity](https://apis.io/arazzos/ankr/ankr-wallet-cross-chain-activity-workflow/)
- [Ankr Wallet Portfolio Snapshot](https://apis.io/arazzos/ankr/ankr-wallet-portfolio-workflow/)

#### AsyncAPI (2)

Event-driven and webhook contracts.

- [Ankr RPC Service — WebSocket Subscriptions](https://apis.io/asyncapis/ankr/ankr-asyncapi/)
- [Review](https://apis.io/asyncapis/ankr/review/)

#### Event channels (4)

Individual events and webhooks the provider emits.

- [/evm/eth_subscribe](https://apis.io/channels/ankr/evm-eth-subscribe/)
- [/evm/eth_unsubscribe](https://apis.io/channels/ankr/evm-eth-unsubscribe/)
- [/solana/subscribe](https://apis.io/channels/ankr/solana-subscribe/)
- [/solana/unsubscribe](https://apis.io/channels/ankr/solana-unsubscribe/)

#### MCP servers (1)

Model Context Protocol servers that expose the API to agents.

- [ankr](https://apis.io/servers/ankr/ankr/)

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Ankr Agentic Access](https://apis.io/agentic-access/ankr/ankr-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Ankr Account Balance](https://apis.io/schemas/ankr/ankr-account-balance/)
- [Ankr NFT Asset](https://apis.io/schemas/ankr/ankr-nft-asset/)
- [Ankr Liquid Staking Metrics](https://apis.io/schemas/ankr/ankr-staking-metrics/)

#### JSON Structure (1)

Data models expressed in JSON Structure.

- [Ankr Account Balance Structure](https://apis.io/json-structure/ankr/ankr-account-balance-structure/)

#### JSON-LD (1)

Linked-data contexts for the provider's vocabulary.

- [Ankr Context](https://apis.io/jsonld/ankr/ankr-context/)

#### Vocabulary (1)

The provider's domain terms, defined.

- [Ankr Vocabulary](https://apis.io/vocabularies/ankr/ankr-vocabulary/)

#### Examples (3)

Example requests and responses.

- [Ankr Eth Rpc Call Example](https://apis.io/examples/ankr/ankr-eth-rpc-call-example/)
- [Ankr Get Account Balance Example](https://apis.io/examples/ankr/ankr-get-account-balance-example/)
- [Ankr Get Nfts By Owner Example](https://apis.io/examples/ankr/ankr-get-nfts-by-owner-example/)

#### Collections (16)

Postman and Open Collection request collections.

- [Ankr Advanced API](https://apis.io/collections/ankr/open-ankr-advanced-api/)
- [Ankr Contract Automation API](https://apis.io/collections/ankr/open-ankr-automation-api/)
- [Ankr Advanced EVM API](https://apis.io/collections/ankr/open-ankr-evm-api/)
- [Ankr Advanced EVM Metrics API](https://apis.io/collections/ankr/open-ankr-metrics-api/)
- [Ankr Advanced EVM NFT API](https://apis.io/collections/ankr/open-ankr-nft-api/)
- [Ankr Advanced EVM Query API](https://apis.io/collections/ankr/open-ankr-query-api/)
- [Ankr Advanced EVM Ratio API](https://apis.io/collections/ankr/open-ankr-ratio-api/)
- [Ankr RPC Service (Node API)](https://apis.io/collections/ankr/open-ankr-rpc-service/)
- [Ankr Liquid Staking API](https://apis.io/collections/ankr/open-ankr-staking-api/)
- [Ankr Advanced EVM Tasks API](https://apis.io/collections/ankr/open-ankr-tasks-api/)
- [Ankr Advanced EVM Token API](https://apis.io/collections/ankr/open-ankr-token-api/)
- [Ankr Advanced EVM Validators API](https://apis.io/collections/ankr/open-ankr-validators-api/)
- [Ankr Advanced API](https://apis.io/collections/ankr/postman-ankr-advanced-api/)
- [Ankr Contract Automation API](https://apis.io/collections/ankr/postman-ankr-automation-api/)
- [Ankr RPC Service (Node API)](https://apis.io/collections/ankr/postman-ankr-rpc-service/)
- [Ankr Liquid Staking API](https://apis.io/collections/ankr/postman-ankr-staking-api/)

#### Governance rules (3)

Spectral rulesets for the provider's contracts.

- [Ankr — asyncapi rules](https://apis.io/rules/ankr/ankr-asyncapi-spectral-rules/)
- [Ankr — jsonschema rules](https://apis.io/rules/ankr/ankr-jsonschema-spectral-rules/)
- [Ankr API Rules](https://apis.io/rules/ankr/ankr-rules/)

#### Security (2)

Authentication, trust centre, and vulnerability disclosure.

- [Ankr Authentication](https://apis.io/security/ankr/ankr-authentication/)
- [Ankr Domain Security](https://apis.io/security/ankr/ankr-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Ankr Plans Pricing](https://apis.io/plans/ankr/ankr-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Ankr Rate Limits](https://apis.io/rate-limits/ankr/ankr-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Ankr Finops](https://apis.io/finops/ankr/ankr-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://www.ankr.com/)
- [Documentation](https://www.ankr.com/docs/)
- [Pricing](https://www.ankr.com/rpc/pricing/)
- [Blog](https://www.ankr.com/blog/)
- [Terms of service](https://www.ankr.com/terms/)
- [Privacy policy](https://www.ankr.com/privacy/)
- [GitHub](https://github.com/Ankr-network)

## API Evangelist rating

**Kin Score 55.6** — strong · rubric 0.25.0 · scored 2026-10-23

| Facet | Score |
|---|---|
| Discoverability | 73.3 |
| Contract quality | 71.3 |
| Contract governance | 27.3 |
| Operational transparency | 13.2 |
| Developer ergonomics | 63.1 |
| Access clarity | 60.5 |

**Agent readiness 44.6** — agent-ready (gated down from agent-native)

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | verified |
| Auth Clarity | served (partial credit) |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | documented (partial credit) |
| Rate Limit Signal | derived (partial credit) |
| Event Surface Described | derived (partial credit) |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | served (partial credit) |
| Protected Resource Metadata | verified |
| Dynamic Client Registration | yes |
| Agentic Commerce | — |
| Pagination Ratio | — |
| Operation Distinctiveness | distinct |

**Regulatory alignment 24.5** — Horizontal (data, software, accessibility, platform)

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/ankr/](https://apis.io/providers/ankr/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Ankr: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/ankr/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
