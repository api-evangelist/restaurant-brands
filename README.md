# Restaurant Brands International (restaurant-brands)

Restaurant Brands International (RBI, NYSE: QSR) is one of the world's largest quick service restaurant companies, with nearly $45 billion in annual system-wide sales and over 32,000 restaurants in more than 120 countries and territories. RBI operates four iconic brands — Tim Hortons, Burger King, Popeyes Louisiana Kitchen, and Firehouse Subs — and in May 2024 closed its $1B acquisition of Carrols Restaurant Group, Burger King's largest U.S. franchisee. RBI Tech Group (rbictg.com) publishes a partner developer portal (the RBI Developer Portal on Confluence) documenting the Partners API — a set of partner-onboarding REST APIs for third-party food ordering marketplaces and POS/kiosk vendors integrating into RBI's fulfillment platform. The documented surface includes ordering (price / commit / fire / place), menu and store retrieval, store-status and order/menu webhooks (Burger King's Partners API v1 "Channel" and v2 "Menu"), loyalty identification and transaction validation, and payment capture / refund endpoints. Access is bilateral: partners request a Staging environment and are issued environment-, country-, and brand-scoped credentials (a bearer JWT for the Partners API; x-region / x-api-key / x-user-datetime headers for the Loyalty middleware). There is no public self-service signup, pricing, or rate card. The public GitHub presence (github.com/rbilabs) is limited to internal tooling forks and an archived hackathon repo.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party

## Tags

- Fortune 500
- Franchising
- Hospitality
- NYSE QSR
- Quick Service Restaurants
- Restaurants

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-06-03

## APIs

### Channel Partners API

Burger King's Partners API v1 — the Channel Partners API for third-party food ordering marketplaces integrating into the Restaurant Brands International (RBI) fulfillment platform. Covers loyalty identification, store and menu retrieval, the order lifecycle (price, commit, fire, place), and order/menu/store webhooks. OpenAPI 3.1.0, bearer JWT auth.

- **Human URL:** [https://bk-partners.rbictg.com/docs/channel/](https://bk-partners.rbictg.com/docs/channel/)
- **Base URL:** `https://bk-partners.rbictg.com/api/v1`

#### Tags

- Ordering
- Loyalty
- Menus
- Stores
- Partner Integration

#### Properties

- [OpenAPI](openapi/channel-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/channel.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/channel.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://bk-partners.rbictg.com/docs/channel/)
- [Documentation](https://rbictg.atlassian.net/wiki/spaces/RDP/pages/4279763050/Partner+API+s)
- [Authentication](https://rbictg.atlassian.net/wiki/spaces/RDP/pages/4963106827/Loyalty+API+-+Getting+Started)
- [J S O N- L D](json-ld/restaurant-brands-channel-context.jsonld)

### Partners Menu API v2

Burger King's Partners API v2 — the Partners Menu API for third-party food ordering marketplaces retrieving store menus from Burger King's end-to-end fulfillment platform. OpenAPI 3.1.0, bearer JWT auth.

- **Human URL:** [https://bk-partners.rbictg.com/docs/v2/](https://bk-partners.rbictg.com/docs/v2/)
- **Base URL:** `https://bk-partners.rbictg.com/api/v2`

#### Tags

- Menus
- Partner Integration

#### Properties

- [OpenAPI](openapi/menu-v2-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/menu-v2.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/menu-v2.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [API Reference](https://bk-partners.rbictg.com/docs/v2/)
- [J S O N- L D](json-ld/restaurant-brands-menu-v2-context.jsonld)

## Common Properties

- [Developer Portal](https://rbictg.atlassian.net/wiki/spaces/RDP/overview)
- [Spectral Rules](rules/restaurant-brands-spectral-rules.yml)
- [Vocabulary](vocabulary/restaurant-brands-vocabulary.yml)
- [Plans](plans/restaurant-brands-plans-pricing.yml)
- [Rate Limits](rate-limits/restaurant-brands-rate-limits.yml)
- [Fin Ops](finops/restaurant-brands-finops.yml)
- [Website](https://www.rbi.com)
- [About](https://www.rbi.com/English/about-us/default.aspx)
- [Investors](https://www.rbi.com/English/investors/default.aspx)
- [News](https://www.rbi.com/English/news/default.aspx)
- [Sustainability](https://www.rbi.com/English/sustainability/default.aspx)
- [Careers](https://careers.rbi.com)
- [LinkedIn](https://www.linkedin.com/company/restaurant-brands-international)
- [Git Hub](https://github.com/rbilabs)
- [S E C  Filings](https://www.rbi.com/English/investors/sec-filings/default.aspx)
- [Burger  King](https://www.bk.com)
- [Tim  Hortons](https://www.timhortons.com)
- [Popeyes](https://www.popeyes.com)
- [Firehouse  Subs](https://www.firehousesubs.com)
- [Carrols  Acquisition](https://www.rbi.com/English/news/news-details/2024/Restaurant-Brands-International-Inc.-Completes-Acquisition-of-Carrols-Restaurant-Group/default.aspx)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
