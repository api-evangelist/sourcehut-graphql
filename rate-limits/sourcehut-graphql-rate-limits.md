# Sourcehut GraphQL Rate Limits

Sourcehut enforces complexity-based rate limiting on its GraphQL API rather
than simple per-request counting. Query complexity is evaluated before execution.

## Complexity Limits

| Constraint          | Default Limit                                  |
|---------------------|------------------------------------------------|
| Query complexity    | 200 (some services may permit higher values)   |
| Max processing time | 3 seconds per standard query                   |
| Pagination default  | 25 results per page                            |

Query complexity is a function of how many resources a request implicates.
Resolvers that accept a `Filter` parameter allow tuning the number of results
returned, which directly affects complexity consumption.

## File Uploads

File upload operations (via the GraphQL multipart request specification) are
granted extended processing time beyond the standard 3-second limit to
accommodate larger payloads.

## Authentication

All requests must be authenticated. Two methods are supported:

- **Personal access tokens** — for CLI tools and scripts
- **OAuth 2.0 bearer tokens** — for third-party applications

Both use the HTTP header: `Authorization: Bearer <token>`

## Pagination

Sourcehut uses cursor-based pagination across all list responses. The default
page size is 25 results. Adjusting page size via `Filter` affects query
complexity and should be tuned carefully against the complexity cap.

Source: https://man.sr.ht/graphql.md
