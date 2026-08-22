# ankr (ankr)

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

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/apis.yml)

## Scope

- **Position:** Consuming

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-29

## APIs

### Ankr RPC Service (Node API)

Ankr's Node API exposes standard JSON-RPC endpoints (HTTPS and WebSocket) for 80+
public blockchains at rpc.ankr.com/{chain}. EVM chains share the Ethereum JSON-RPC envelope;
non-EVM chains (Solana, Aptos, TRON, Stellar, TON, Cosmos networks) expose their native
RPC surface at the same per-chain endpoint. Public Plan is open and anonymous;
Premium Plan multiplies throughput x50 and unlocks WebSocket subscriptions, archive nodes,
and IP whitelisting via project-scoped API keys.

- **Human URL:** [https://www.ankr.com/rpc/](https://www.ankr.com/rpc/)
- **Base URL:** `https://rpc.ankr.com`

#### Tags

- RPC
- Web3
- Multichain
- EVM
- Blockchain

#### Properties

- [Documentation](https://www.ankr.com/docs/rpc-service/overview/)
- [Documentation](https://www.ankr.com/docs/rpc-service/chains/chains-list/)
- [OpenAPI](openapi/ankr-rpc-service-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ankr-rpc-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-rpc-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [AsyncAPI](asyncapi/ankr-asyncapi.yml) — [AsyncAPI Specification](https://www.asyncapi.com/docs/reference/specification/latest)
- [JSON-LD](json-ld/ankr-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)

### Ankr Advanced API

The Advanced API (AAPI) is Ankr's indexed JSON-RPC surface that optimizes, caches, and
aggregates data across 19 EVM mainnets and 7 testnets. Methods are grouped into NFT
(ankr_getNFTsByOwner, ankr_getNFTMetadata, ankr_getNFTHolders, ankr_getNftTransfers),
Token (ankr_getAccountBalance, ankr_getCurrencies, ankr_getTokenPrice, ankr_getTokenHolders,
ankr_getTokenHoldersCount, ankr_getTokenTransfers, ankr_getTokenPriceHistory), and Query
(ankr_getBlockchainStats, ankr_getBlocks, ankr_getLogs, ankr_getTransactionsByHash,
ankr_getTransactionsByAddress, ankr_getInteractions).

- **Human URL:** [https://www.ankr.com/docs/advanced-api/overview/](https://www.ankr.com/docs/advanced-api/overview/)
- **Base URL:** `https://rpc.ankr.com/multichain`

#### Tags

- Web3
- NFT
- Token
- Indexer
- Multichain

#### Properties

- [Documentation](https://www.ankr.com/docs/advanced-api/overview/)
- [Documentation](https://api-docs.ankr.com/reference/)
- [OpenAPI](openapi/ankr-advanced-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ankr-advanced-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-advanced-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ankr-nft-asset-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/ankr-account-balance-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/ankr-account-balance-structure.json)
- [Example](examples/ankr-get-account-balance-example.json)
- [Example](examples/ankr-get-nfts-by-owner-example.json)

### Ankr Liquid Staking API

Ankr's Liquid Staking developer surface — a RESTful metrics API plus on-chain Smart Contract
APIs across Avalanche, Binance Smart Chain, Ethereum, Fantom, and Polygon. Supported
liquid staking tokens include ankrETH, ankrBNB, ankrPOL, ankrAVAX, ankrFTM, ankrDOT, and
ankrFLOW. The RESTful surface exposes staking metrics (TVL, APR, holders, supply),
the trustless exchange ratio, and validator metadata (unbond windows, reward release).

- **Human URL:** [https://www.ankr.com/docs/staking-for-developers/overview/](https://www.ankr.com/docs/staking-for-developers/overview/)
- **Base URL:** `https://api.staking.ankr.com`

#### Tags

- Staking
- LiquidStaking
- DeFi
- Validators

#### Properties

- [Documentation](https://www.ankr.com/docs/staking-for-developers/overview/)
- [OpenAPI](openapi/ankr-staking-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ankr-staking-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-staking-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [JSON Schema](json-schema/ankr-staking-metrics-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [Dashboard](https://www.ankr.com/staking/dashboard/)

### Ankr Contract Automation API

Ankr Contract Automation executes deployed smart-contract functions based on time-based (CRON)
or event-driven (IAutomateCompatible) triggers. As of May 2026 the service supports BNB Smart Chain
only — additional networks are on the roadmap. Tasks are created, funded, paused, and deleted via
the Ankr Automation Dashboard.

- **Human URL:** [https://www.ankr.com/docs/automation/overview/](https://www.ankr.com/docs/automation/overview/)
- **Base URL:** `https://www.ankr.com/automation`

#### Tags

- Automation
- SmartContracts
- BNB

#### Properties

- [Documentation](https://www.ankr.com/docs/automation/overview/)
- [OpenAPI](openapi/ankr-automation-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/ankr-automation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-automation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

### AnkrScan Block Explorer

AnkrScan is Ankr's multi-chain block explorer covering EVM and non-EVM networks. It is a hosted
UI consuming Ankr's Node API and Advanced API and does not currently publish a public REST surface.

- **Human URL:** [https://ankrscan.io](https://ankrscan.io)
- **Base URL:** `https://ankrscan.io`

#### Tags

- BlockExplorer
- Web3

#### Properties

- [Portal](https://ankrscan.io)
- [Postman Collection](collections/ankr-advanced-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-advanced-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ankr-automation-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-automation-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ankr-rpc-service.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-rpc-service.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Postman Collection](collections/ankr-staking-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/ankr-staking-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)

## Common Properties

- [Arazzo Workflows](arazzo/) — [Arazzo Specification](https://spec.openapis.org/arazzo/latest.html)
- [Portal](https://www.ankr.com)
- [Documentation](https://www.ankr.com/docs/)
- [Sign Up](https://www.ankr.com/rpc/)
- [Dashboard](https://www.ankr.com/rpc/projects/)
- [Pricing](https://www.ankr.com/rpc/pricing/)
- [Blog](https://www.ankr.com/blog/)
- [Company](https://www.ankr.com/about/)
- [Twitter](https://x.com/ankr)
- [Forum](https://discord.com/invite/ankrnetwork)
- [Forum](https://t.me/ankrnetwork)
- [GitHub Organization](https://github.com/Ankr-network)
- [SDK](https://github.com/Ankr-network/ankr.js)
- [SDK](https://github.com/Ankr-network/ankr-python-sdk)
- [SDK](https://github.com/Ankr-network/ankr-sdk-nodejs)
- [SDK](https://github.com/Ankr-network/game-unity-sdk)
- [SDK](https://github.com/Ankr-network/game-unreal-sdk)
- [SDK](https://github.com/Ankr-network/game-unreal-aptos-sdk)
- [SDK](https://github.com/Ankr-network/ankr-compound-sdk)
- [SDK](https://github.com/Ankr-network/ankrscan-sdk)
- [C L I](https://github.com/Ankr-network/ankr-cli)
- [Source Code](https://github.com/Ankr-network/ankr-docs)
- [Source Code](https://github.com/Ankr-network/erigon)
- [Block Explorer](https://ankrscan.io)
- [Documentation](https://api-docs.ankr.com/reference/)
- [Documentation](https://api-docs.ankr.com/llms.txt)
- [Status](https://status.ankr.com)
- [Terms of Service](https://www.ankr.com/terms/)
- [Privacy Policy](https://www.ankr.com/privacy/)
- [Plans](plans/ankr-plans-pricing.yml)
- [Rate Limits](rate-limits/ankr-rate-limits.yml)
- [Fin Ops](finops/ankr-finops.yml)
- [Vocabulary](vocabulary/ankr-vocabulary.yml)
- [Spectral Rules](rules/ankr-rules.yml)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** info@apievangelist.com
**URL:** https://apievangelist.com
