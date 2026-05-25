# Ankr (ankr)

Ankr is a Web3 infrastructure provider whose multichain RPC, Advanced API, liquid staking, contract automation, and Rollup-as-a-Service products serve developers, exchanges, and enterprises across 80+ blockchains. The Node API exposes JSON-RPC and WebSocket endpoints at `rpc.ankr.com/{chain}`; the Advanced API (AAPI) layers an indexed query surface across 19 EVM mainnets for NFT, token, and historical-data reads. Ankr also operates liquid staking pools (ankrETH, ankrBNB, ankrPOL, ankrAVAX, ankrFTM, ankrDOT, ankrFLOW), a contract automation service on BNB Smart Chain, and an enterprise Rollup-as-a-Service practice that supports OP Stack, Polygon CDK, and Arbitrum Orbit variants. Infrastructure runs as a global DePIN of bare-metal nodes in 30+ regions serving roughly 8 billion daily RPC requests.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/ankr/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- RPC, Web3, Multichain, EVM, NFT, Token, Staking, LiquidStaking, Automation, Blockchain, DePIN, Indexer

## Timestamps

- **Created:** 2026-05-25
- **Modified:** 2026-05-25

## APIs

### Ankr RPC Service (Node API)
JSON-RPC and WebSocket endpoints for 80+ blockchains at `rpc.ankr.com/{chain}`. Public Plan is free and anonymous; Premium Plan multiplies Node API throughput x50 with project-scoped API keys, archive nodes, WSS, and IP whitelisting.

**Human URL:** [https://www.ankr.com/rpc/](https://www.ankr.com/rpc/)

- [Documentation](https://www.ankr.com/docs/rpc-service/overview/)
- [Documentation — Chains list](https://www.ankr.com/docs/rpc-service/chains/chains-list/)
- [OpenAPI](openapi/ankr-rpc-service-openapi.yml)
- [JSON-LD](json-ld/ankr-context.jsonld)
- [Naftiko Capability — EVM RPC](capabilities/rpc-service-evm.yaml)

### Ankr Advanced API
Indexed JSON-RPC surface (`ankr_*` methods) across 19 EVM mainnets and 7 testnets, grouped into NFT, Token, and Query categories. Multichain endpoint at `rpc.ankr.com/multichain/{API_KEY}`.

**Human URL:** [https://www.ankr.com/docs/advanced-api/overview/](https://www.ankr.com/docs/advanced-api/overview/)

- [Documentation](https://www.ankr.com/docs/advanced-api/overview/)
- [API Reference](https://api-docs.ankr.com/reference/)
- [OpenAPI](openapi/ankr-advanced-api-openapi.yml)
- [JSON Schema — NFT Asset](json-schema/ankr-nft-asset-schema.json)
- [JSON Schema — Account Balance](json-schema/ankr-account-balance-schema.json)
- [JSON Structure — Account Balance](json-structure/ankr-account-balance-structure.json)
- [Example — Get Account Balance](examples/ankr-get-account-balance-example.json)
- [Example — Get NFTs By Owner](examples/ankr-get-nfts-by-owner-example.json)
- [Naftiko Capability — NFT](capabilities/advanced-api-nft.yaml)
- [Naftiko Capability — Token](capabilities/advanced-api-token.yaml)
- [Naftiko Capability — Query](capabilities/advanced-api-query.yaml)

### Ankr Liquid Staking API
RESTful metrics for Ankr's liquid staking pools (ankrETH, ankrBNB, ankrPOL, ankrAVAX, ankrFTM, ankrDOT, ankrFLOW) plus on-chain Smart Contract APIs on Avalanche, BSC, Ethereum, Fantom, and Polygon.

**Human URL:** [https://www.ankr.com/docs/staking-for-developers/overview/](https://www.ankr.com/docs/staking-for-developers/overview/)

- [Documentation](https://www.ankr.com/docs/staking-for-developers/overview/)
- [OpenAPI](openapi/ankr-staking-api-openapi.yml)
- [JSON Schema — Staking Metrics](json-schema/ankr-staking-metrics-schema.json)
- [Naftiko Capability — Staking Metrics](capabilities/staking-metrics.yaml)
- [Dashboard — Staking](https://www.ankr.com/staking/dashboard/)

### Ankr Contract Automation API
Time-based (CRON) and event-driven (IAutomateCompatible) execution of smart-contract functions. BNB Smart Chain only as of May 2026.

**Human URL:** [https://www.ankr.com/docs/automation/overview/](https://www.ankr.com/docs/automation/overview/)

- [Documentation](https://www.ankr.com/docs/automation/overview/)
- [OpenAPI](openapi/ankr-automation-api-openapi.yml)
- [Naftiko Capability — Automation Tasks](capabilities/automation-tasks.yaml)

### AnkrScan Block Explorer
Multichain block explorer UI at ankrscan.io. Consumes Ankr's Node API and Advanced API; no public REST surface.

**Human URL:** [https://ankrscan.io](https://ankrscan.io)

## Common Properties

- [Portal — ankr.com](https://www.ankr.com)
- [Documentation — docs](https://www.ankr.com/docs/)
- [Documentation — API Reference](https://api-docs.ankr.com/reference/)
- [Documentation — llms.txt index](https://api-docs.ankr.com/llms.txt)
- [SignUp — Web3 platform](https://www.ankr.com/rpc/)
- [Dashboard — Projects](https://www.ankr.com/rpc/projects/)
- [Pricing](https://www.ankr.com/rpc/pricing/)
- [Blog](https://www.ankr.com/blog/)
- [Company — About](https://www.ankr.com/about/)
- [Twitter — @ankr](https://x.com/ankr)
- [Forum — Discord](https://discord.com/invite/ankrnetwork)
- [Forum — Telegram](https://t.me/ankrnetwork)
- [GitHubOrganization — Ankr-network](https://github.com/Ankr-network)
- [SDK — ankr.js (TypeScript)](https://github.com/Ankr-network/ankr.js)
- [SDK — ankr-python-sdk](https://github.com/Ankr-network/ankr-python-sdk)
- [SDK — ankr-sdk-nodejs](https://github.com/Ankr-network/ankr-sdk-nodejs)
- [SDK — Mirage Unity SDK](https://github.com/Ankr-network/game-unity-sdk)
- [SDK — Mirage Unreal SDK](https://github.com/Ankr-network/game-unreal-sdk)
- [SDK — Mirage Unreal Aptos SDK](https://github.com/Ankr-network/game-unreal-aptos-sdk)
- [SDK — Compound SDK](https://github.com/Ankr-network/ankr-compound-sdk)
- [SDK — AnkrScan Go SDK](https://github.com/Ankr-network/ankrscan-sdk)
- [CLI — ankr-cli](https://github.com/Ankr-network/ankr-cli)
- [SourceCode — ankr-docs](https://github.com/Ankr-network/ankr-docs)
- [SourceCode — Erigon fork](https://github.com/Ankr-network/erigon)
- [BlockExplorer — AnkrScan](https://ankrscan.io)
- [Status](https://status.ankr.com)
- [TermsOfService](https://www.ankr.com/terms/)
- [PrivacyPolicy](https://www.ankr.com/privacy/)
- [Plans](plans/ankr-plans-pricing.yml)
- [RateLimits](rate-limits/ankr-rate-limits.yml)
- [FinOps](finops/ankr-finops.yml)
- [Vocabulary](vocabulary/ankr-vocabulary.yml)
- [SpectralRules](rules/ankr-rules.yml)

## Features

- 80+ blockchain networks behind a single multichain RPC surface (`rpc.ankr.com/{chain}`)
- Average response time of 56ms with claimed 99.99% uptime across a 30+ region DePIN
- 8 billion daily RPC requests served as of May 2026
- Public Plan free with anonymous IP-scoped throttling — production should use Premium
- Premium Plan multiplies Node API throughput x50 and Advanced API x30
- WebSocket (WSS) endpoints, archive access, IP whitelisting, multi-project statistics
- Advanced API — indexed JSON-RPC over 19 EVM mainnets exposing NFT, Token, Query methods
- `ankr_getAccountBalance` returns native + ERC-20 balances across multiple chains in one call
- NFT methods — `ankr_getNFTsByOwner`, `ankr_getNFTMetadata`, `ankr_getNFTHolders`, `ankr_getNftTransfers`
- Pricing methods — `ankr_getTokenPrice`, `ankr_getTokenPriceHistory` (no third-party oracle required)
- Query methods — `ankr_getLogs`, `ankr_getTransactionsByAddress`, `ankr_getInteractions`
- Liquid staking on 7+ chains via ankrETH, ankrBNB, ankrPOL, ankrAVAX, ankrFTM, ankrDOT, ankrFLOW
- Liquid Staking RESTful metrics API at `https://api.staking.ankr.com/v1.0/metrics`
- Trustless ratio oracles and PancakeSwap price oracle for `ankr*` tokens
- Smart Contract Automation on BNB Smart Chain with CRON and event triggers
- Rollup-as-a-Service (RaaS) — OP Stack, Polygon CDK, Arbitrum Orbit, custom appchains
- Bitcoin Secured Infrastructure for chains anchoring security to Bitcoin
- Enterprise DVN infrastructure on LayerZero for cross-chain messaging
- Recent RPC launches — HyperEVM, Unichain, AB Chain, Kite (AI Payment Blockchain)
- Powers AI/blockchain integrations including ChainGPT AI Hub V2 (March 2026)
- SDKs — ankr.js (TypeScript), ankr-python-sdk, Mirage Unity SDK, Mirage Unreal SDK
- AnkrScan multi-chain block explorer at ankrscan.io
- Open-source Erigon and BSC-Erigon forks operated for archive workloads

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Ankr RPC Service](openapi/ankr-rpc-service-openapi.yml)
- [Ankr Advanced API](openapi/ankr-advanced-api-openapi.yml)
- [Ankr Liquid Staking API](openapi/ankr-staking-api-openapi.yml)
- [Ankr Contract Automation API](openapi/ankr-automation-api-openapi.yml)

### JSON Schema

- [Ankr NFT Asset](json-schema/ankr-nft-asset-schema.json)
- [Ankr Account Balance](json-schema/ankr-account-balance-schema.json)
- [Ankr Staking Metrics](json-schema/ankr-staking-metrics-schema.json)

### JSON Structure

- [Ankr Account Balance Structure](json-structure/ankr-account-balance-structure.json)

### JSON-LD

- [Ankr Context](json-ld/ankr-context.jsonld)

### Capabilities (Naftiko)

- [Advanced API — NFT](capabilities/advanced-api-nft.yaml)
- [Advanced API — Token](capabilities/advanced-api-token.yaml)
- [Advanced API — Query](capabilities/advanced-api-query.yaml)
- [RPC Service — EVM](capabilities/rpc-service-evm.yaml)
- [Staking — Metrics](capabilities/staking-metrics.yaml)
- [Automation — Tasks](capabilities/automation-tasks.yaml)

### Examples

- [Get Account Balance](examples/ankr-get-account-balance-example.json)
- [Get NFTs By Owner](examples/ankr-get-nfts-by-owner-example.json)
- [eth_blockNumber RPC Call](examples/ankr-eth-rpc-call-example.json)

### Rules

- [Ankr Spectral Rules](rules/ankr-rules.yml)

### Plans / Rate Limits / FinOps

- [Plans](plans/ankr-plans-pricing.yml)
- [Rate Limits](rate-limits/ankr-rate-limits.yml)
- [FinOps](finops/ankr-finops.yml)

### Vocabulary

- [Ankr Vocabulary](vocabulary/ankr-vocabulary.yml)

## Maintainers

- Kin Lane — [apievangelist.com](https://apievangelist.com) — info@apievangelist.com
