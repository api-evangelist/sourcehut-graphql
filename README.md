# Sourcehut GraphQL

Sourcehut (sr.ht) is an open-source software forge offering version control,
build automation, bug tracking, mailing lists, and more through a unified
GraphQL API. Each service exposes its own GraphQL endpoint at /query, enabling
developers to query and manage their projects programmatically with a consistent
interface.

## Links

- **Website:** https://sourcehut.org/
- **API Documentation:** https://man.sr.ht/graphql.md
- **GraphQL Endpoints:** https://git.sr.ht/query, https://builds.sr.ht/query, etc.
- **GitHub Organization:** https://github.com/sourcehut
- **Pricing:** https://sourcehut.org/pricing/

## GraphQL Endpoints

| Service         | Endpoint                        |
|-----------------|---------------------------------|
| git.sr.ht       | https://git.sr.ht/query         |
| builds.sr.ht    | https://builds.sr.ht/query      |
| hg.sr.ht        | https://hg.sr.ht/query          |
| lists.sr.ht     | https://lists.sr.ht/query       |
| meta.sr.ht      | https://meta.sr.ht/query        |
| paste.sr.ht     | https://paste.sr.ht/query       |
| todo.sr.ht      | https://todo.sr.ht/query        |

## Authentication

All API requests require authentication via:
- Personal access tokens (`Authorization: Bearer <token>`)
- OAuth 2.0 bearer tokens

## Rate Limits

- Query complexity cap: 200 (default)
- Max processing time: 3 seconds
- Pagination default: 25 results per page

## Pricing

Sourcehut uses a pay-what-you-can model with three tiers ($4, $8, $12/month),
all providing identical API access. Financial aid is available.
