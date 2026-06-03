# Restaurant Brands International (restaurant-brands)

Restaurant Brands International (RBI, NYSE: QSR) is one of the world's largest quick service restaurant companies, with nearly $45 billion in annual system-wide sales and over 32,000 restaurants in more than 120 countries and territories. RBI operates four iconic brands — Tim Hortons, Burger King, Popeyes Louisiana Kitchen, and Firehouse Subs — and in May 2024 closed its $1B acquisition of Carrols Restaurant Group, Burger King's largest U.S. franchisee. RBI Tech Group (rbictg.com) publishes a partner developer portal (the RBI Developer Portal on Confluence) documenting the Partners API — a set of partner-onboarding REST APIs for third-party food ordering marketplaces and POS/kiosk vendors integrating into RBI's fulfillment platform. The documented surface includes ordering (price / commit / fire / place), menu and store retrieval, store-status and order/menu webhooks (Burger King's Partners API v1 "Channel" and v2 "Menu"), loyalty identification and transaction validation, and payment capture / refund endpoints. Access is bilateral: partners request a Staging environment and are issued environment-, country-, and brand-scoped credentials (a bearer JWT for the Partners API; x-region / x-api-key / x-user-datetime headers for the Loyalty middleware). There is no public self-service signup, pricing, or rate card. The public GitHub presence (github.com/rbilabs) is limited to internal tooling forks and an archived hackathon repo.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags:

 - Fortune 500, Franchising, Hospitality, NYSE QSR, Quick Service Restaurants, Restaurants

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-06-03

## APIs

### Channel Partners API

Burger King's Partners API v1 — the Channel Partners API for third-party food ordering marketplaces integrating into the Restaurant Brands International (RBI) fulfillment platform. Covers loyalty identification, store and menu retrieval, the order lifecycle (price, commit, fire, place), and order/menu/store webhooks. OpenAPI 3.1.0, bearer JWT auth.

**Human URL:** [https://bk-partners.rbictg.com/docs/channel/](https://bk-partners.rbictg.com/docs/channel/)

**Base URL:** `https://bk-partners.rbictg.com/api/v1`

#### Tags:

 - Ordering, Loyalty, Menus, Stores, Partner Integration

#### Properties

- [OpenAPI](openapi/channel-openapi.yml)
- [APIReference](https://bk-partners.rbictg.com/docs/channel/)
- [Documentation](https://rbictg.atlassian.net/wiki/spaces/RDP/pages/4279763050/Partner+API+s)
- [Authentication](https://rbictg.atlassian.net/wiki/spaces/RDP/pages/4963106827/Loyalty+API+-+Getting+Started)
- [JSON-LD](json-ld/restaurant-brands-channel-context.jsonld)
- [NaftikoCapability](capabilities/channel-loyalty.yaml)
- [NaftikoCapability](capabilities/channel-menus.yaml)
- [NaftikoCapability](capabilities/channel-orders.yaml)
- [NaftikoCapability](capabilities/channel-stores.yaml)

### Partners Menu API v2

Burger King's Partners API v2 — the Partners Menu API for third-party food ordering marketplaces retrieving store menus from Burger King's end-to-end fulfillment platform. OpenAPI 3.1.0, bearer JWT auth.

**Human URL:** [https://bk-partners.rbictg.com/docs/v2/](https://bk-partners.rbictg.com/docs/v2/)

**Base URL:** `https://bk-partners.rbictg.com/api/v2`

#### Tags:

 - Menus, Partner Integration

#### Properties

- [OpenAPI](openapi/menu-v2-openapi.yml)
- [APIReference](https://bk-partners.rbictg.com/docs/v2/)
- [JSON-LD](json-ld/restaurant-brands-menu-v2-context.jsonld)
- [NaftikoCapability](capabilities/menu-v2-menus.yaml)

## Common Properties

- [Developer Portal](https://rbictg.atlassian.net/wiki/spaces/RDP/overview)
- [Spectral Rules](rules/restaurant-brands-spectral-rules.yml)
- [Vocabulary](vocabulary/restaurant-brands-vocabulary.yml)
- [Plans](plans/restaurant-brands-plans-pricing.yml)
- [Rate Limits](rate-limits/restaurant-brands-rate-limits.yml)
- [FinOps](finops/restaurant-brands-finops.yml)
- [Website](https://www.rbi.com)
- [About](https://www.rbi.com/English/about-us/default.aspx)
- [Investors](https://www.rbi.com/English/investors/default.aspx)
- [News](https://www.rbi.com/English/news/default.aspx)
- [Sustainability](https://www.rbi.com/English/sustainability/default.aspx)
- [Careers](https://careers.rbi.com)
- [LinkedIn](https://www.linkedin.com/company/restaurant-brands-international)
- [GitHub](https://github.com/rbilabs)
- [SEC Filings](https://www.rbi.com/English/investors/sec-filings/default.aspx)
- [Carrols Acquisition](https://www.rbi.com/English/news/news-details/2024/Restaurant-Brands-International-Inc.-Completes-Acquisition-of-Carrols-Restaurant-Group/default.aspx)

## Brands

- [Burger King](https://www.bk.com)
- [Tim Hortons](https://www.timhortons.com)
- [Popeyes](https://www.popeyes.com)
- [Firehouse Subs](https://www.firehousesubs.com)

## Artifacts

Machine-readable API specifications organized by format.

### OpenAPI

- [Burger King's Partners API (Channel, v1)](openapi/channel-openapi.yml) — 10 operations, 3 webhooks, 84 schemas
- [Burger King's Partners API v2 (Menu)](openapi/menu-v2-openapi.yml) — 2 operations, 24 schemas

### JSON Schema

- 106 JSON Schema files in [`json-schema/`](json-schema/) extracted from the Channel (v1) and Menu (v2) component schemas.

### JSON Structure

- 106 JSON Structure files in [`json-structure/`](json-structure/) converted from the JSON Schema set.

### JSON-LD

- [restaurant-brands-channel-context.jsonld](json-ld/restaurant-brands-channel-context.jsonld)
- [restaurant-brands-menu-v2-context.jsonld](json-ld/restaurant-brands-menu-v2-context.jsonld)

### Examples

- 106 example payloads in [`examples/`](examples/), one per JSON Schema.

## Capabilities

Self-contained Naftiko capabilities, one per OpenAPI tag, each exposing a REST adapter and an MCP adapter routed through its own inline consumes block.

| Workflow | API | Tools | Persona |
|----------|-----|-------|---------|
| [Channel — Loyalty](capabilities/channel-loyalty.yaml) | Channel Partners API | 1 | Partner Integrator |
| [Channel — Menus](capabilities/channel-menus.yaml) | Channel Partners API | 1 | Partner Integrator |
| [Channel — Orders](capabilities/channel-orders.yaml) | Channel Partners API | 5 | Partner Integrator |
| [Channel — Stores](capabilities/channel-stores.yaml) | Channel Partners API | 3 | Partner Integrator |
| [Menu v2 — Menus](capabilities/menu-v2-menus.yaml) | Partners Menu API v2 | 2 | Partner Integrator |

## Vocabulary

- [Restaurant Brands International Vocabulary](vocabulary/restaurant-brands-vocabulary.yml) — Unified taxonomy mapping 3 resources, 7 actions, 5 workflows, and 2 personas across operational (OpenAPI) and capability (Naftiko) dimensions.

## Rules

- [Restaurant Brands Spectral Rules](rules/restaurant-brands-spectral-rules.yml) — 23 rules across info, servers, paths, operations, parameters, responses, security, schema, and quality categories enforcing RBI Partners API conventions.

## Plans, Rate Limits & FinOps

- [Plans / Pricing](plans/restaurant-brands-plans-pricing.yml) — Partner onboarding model (bilateral, contact sales; not publicly priced).
- [Rate Limits](rate-limits/restaurant-brands-rate-limits.yml) — Credential-scoped; numeric thresholds not publicly documented.
- [FinOps](finops/restaurant-brands-finops.yml) — FOCUS-aligned meters for orders, menu/store syncs, loyalty identifications, and payment captures.

## Public GitHub presence (rbilabs)

14 public repos, all internal tooling forks or archived (no published SDKs or API clients for third parties): `graphql-schema-utilities`, `ncr-bsp-hmac` (HMAC sample for NCR BSP POS APIs), `apollo-server-cache-dynamodb`, `aws-api-gateway-developer-portal` (archived), `cypress-autorecord`, `jira-pr-link-action`, `slack-orb`, `capacitor`, `react-dfp`, `metricslib`, `deploy-sourcegraph-docker`, `javascript`, `wyncode-hackathon` (archived), `dummy-repo` (archived). No MCP servers or Claude Code skills are published by RBI.

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
