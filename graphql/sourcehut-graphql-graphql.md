# Sourcehut GraphQL GraphQL API

The Sourcehut (sr.ht) GraphQL API provides programmatic access to the git.sr.ht version control service. It exposes types for repositories, git objects (commits, trees, blobs, tags), references, access control lists, deploy keys, artifacts, and webhook subscriptions. Authentication is required via a personal access token or OAuth 2.0 Bearer token. The API enforces OAuth 2.0 access scopes (PROFILE, REPOSITORIES, OBJECTS, ACLS) with read/write granularity. Query complexity is capped at 200 by default and processing time is limited to 3 seconds per request. Cursor-based pagination is used throughout. File uploads are supported via the multipart request spec.

**Endpoint:** https://git.sr.ht/query

**Documentation:** https://man.sr.ht/graphql.md

**References:**

- Documentation: https://man.sr.ht/graphql.md
- GettingStarted: https://man.sr.ht/graphql.md
- GitHub: https://git.sr.ht/~sircmpwn/git.sr.ht
