# ankr (ankr)

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
