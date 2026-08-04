# Sourcehut GraphQL

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
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
