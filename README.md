# DoltHub (dolthub)

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

DoltHub is the hosting platform for Dolt, the version-controlled SQL database - "Git for data". DoltHub hosts public and private Dolt databases and exposes an HTTP API (the DoltHub SQL API) for running read and write SQL queries against any branch, plus repository, branch, tag, fork, and asynchronous job/operation management over a Git-style version-controlled MySQL-compatible database.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/dolthub/refs/heads/main/apis.yml)

## Tags

- Database
- SQL
- Version Control
- Git for Data
- MySQL

## Timestamps

- **Created:** 2026-06-20
- **Modified:** 2026-06-20

## APIs

### DoltHub SQL Query API

Read-only SQL query endpoint that executes a SELECT (or other read) query against any owner/database/branch on DoltHub and returns a JSON response containing the schema, rows, and query execution status.

- **Human URL:** [https://docs.dolthub.com/products/dolthub/api/sql](https://docs.dolthub.com/products/dolthub/api/sql)
- **Base URL:** `https://www.dolthub.com/api/v1alpha1`

#### Tags

- SQL
- Query
- Read

#### Properties

- [Documentation](https://docs.dolthub.com/products/dolthub/api/sql)
- [API Reference](https://docs.dolthub.com/products/dolthub/api/sql)
- [OpenAPI](openapi/dolthub-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dolthub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [GitHub](https://github.com/dolthub/dolt)

### DoltHub Write API

Asynchronous write endpoint that executes INSERT / UPDATE / DELETE SQL against a destination branch (created from a source branch if missing) and returns an operation name to poll for completion and the resulting commit IDs. Requires a Bearer / token authorization header.

- **Human URL:** [https://docs.dolthub.com/products/dolthub/api/sql](https://docs.dolthub.com/products/dolthub/api/sql)
- **Base URL:** `https://www.dolthub.com/api/v1alpha1`

#### Tags

- SQL
- Write
- Async

#### Properties

- [Documentation](https://docs.dolthub.com/products/dolthub/api/sql)
- [API Reference](https://www.dolthub.com/blog/2022-01-12-sql-api-writes/)
- [OpenAPI](openapi/dolthub-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dolthub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [GitHub](https://github.com/dolthub/dolt)

### DoltHub Repositories and Branches API

Version-control management endpoints for creating databases, forking databases, listing forks, creating and listing branches and tags, and polling asynchronous jobs and operations on a Dolt database.

- **Human URL:** [https://docs.dolthub.com/products/dolthub/api/database](https://docs.dolthub.com/products/dolthub/api/database)
- **Base URL:** `https://www.dolthub.com/api/v1alpha1`

#### Tags

- Repositories
- Branches
- Tags
- Forks

#### Properties

- [Documentation](https://docs.dolthub.com/products/dolthub/api/database)
- [API Reference](https://www.dolthub.com/blog/2023-02-24-introducing-the-new-dolthub-api/)
- [OpenAPI](openapi/dolthub-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/dolthub.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [GitHub](https://github.com/dolthub/dolt)

### Dolt SQL Server

The open-source Dolt database ships a MySQL-compatible SQL server (dolt sql-server) over the MySQL wire protocol, giving the same versioned database hosted on DoltHub a self-hostable, drop-in SQL interface for any MySQL client or driver.

- **Human URL:** [https://docs.dolthub.com/sql-reference/server/sql-server](https://docs.dolthub.com/sql-reference/server/sql-server)
- **Base URL:** `https://github.com/dolthub/dolt`

#### Tags

- Dolt
- MySQL
- SQL Server

#### Properties

- [Documentation](https://docs.dolthub.com/sql-reference/server/sql-server)
- [GitHub](https://github.com/dolthub/dolt)

## Common Properties

- [GitHub Organization](https://github.com/dolthub)
- [LinkedIn](https://www.linkedin.com/company/dolthub)
- [Website](https://www.dolthub.com)
- [Documentation](https://docs.dolthub.com)
- [Plans](plans/dolthub-plans-pricing.yml)
- [Rate Limits](rate-limits/dolthub-rate-limits.yml)
- [Fin Ops](finops/dolthub-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
