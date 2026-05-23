# Restaurant Brands International (restaurant-brands)

Restaurant Brands International (RBI, NYSE: QSR) is one of the world's largest quick service restaurant companies, with nearly $45 billion in annual system-wide sales and over 32,000 restaurants in more than 120 countries and territories. RBI operates four iconic brands — Tim Hortons, Burger King, Popeyes Louisiana Kitchen, and Firehouse Subs — and in May 2024 closed its $1B acquisition of Carrols Restaurant Group, Burger King's largest U.S. franchisee. RBI publishes no public developer program; its consumer ordering, loyalty (Royal Perks, Tims Rewards, Popeyes Rewards, Firehouse Rewards), and franchisee/POS surfaces run on a private GraphQL backend operated by RBI Tech Group (rbictg.com) and integrate with NCR Voyix BSP POS APIs via HMAC. The public-facing GitHub presence (github.com/rbilabs) is limited to internal tooling forks (GraphQL schema utilities, Apollo Server DynamoDB cache, AWS API Gateway Developer Portal, Cypress autorecord, Jira PR link action) and an archived hackathon repo.

**URL:** [Visit APIs.json URL](https://raw.githubusercontent.com/api-evangelist/restaurant-brands/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Consuming
- **Access:** 3rd-Party
- **xType:** company
- **xTier:** 3 (no-apis)

## Tags

Fortune 500, Franchising, Hospitality, NYSE QSR, Quick Service Restaurants, Restaurants

## Timestamps

- **Created:** 2026-05-23
- **Modified:** 2026-05-23

## APIs

No public developer APIs are published by Restaurant Brands International or its operating brands. The private consumer-app backend (use1-prod-bk.rbictg.com/graphql and sibling deployments per brand) returns HTTP 401 to unauthenticated clients and is not documented for third-party use. POS integration is handled internally against NCR Voyix BSP APIs (see rbilabs/ncr-bsp-hmac for the HMAC code sample). Delivery and aggregator integration is handled bilaterally with DoorDash, Uber Eats, Skip the Dishes, and similar partners — not via an RBI-exposed API.

## Brands

- [Burger King](https://www.bk.com)
- [Tim Hortons](https://www.timhortons.com)
- [Popeyes](https://www.popeyes.com)
- [Firehouse Subs](https://www.firehousesubs.com)

## Public GitHub presence (rbilabs)

14 public repos, all internal tooling (no published SDKs or API clients for third parties):

- `graphql-schema-utilities` — CLI to merge GraphQL schemas (published to npm)
- `apollo-server-cache-dynamodb` — Apollo Server cache backed by DynamoDB
- `ncr-bsp-hmac` — Java sample for HMAC-signed NCR BSP POS API calls
- `aws-api-gateway-developer-portal` — fork of awslabs serverless dev portal (archived Feb 2024)
- `cypress-autorecord`, `jira-pr-link-action`, `slack-orb`, `capacitor`, `react-dfp`, `metricslib`, `deploy-sourcegraph-docker`, `javascript`, `wyncode-hackathon`, `dummy-repo`

## Common Properties

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

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
