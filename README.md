# DoltHub (dolthub)

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
