#### Title: Create Post Timescale dbt Model in Silver Layer

#### Description
As a Data Engineer, I want to pivot and transform post data from the TimescaleDB source into the Silver layer, So that we can compare it with Apify metrics to find and resolve data discrepancies.

#### Background
This task is part of the effort to reconcile data between TimescaleDB and Apify sources. It depends on the completion of [NXS-492](https://unitedtalent.atlassian.net/browse/NXS-492), which involves migrating historical TimescaleDB data into the Bronze layer. This ticket is **BLOCKED** until NXS-492 is resolved. The affected platforms include TimescaleDB, Snowflake, and dbt.

#### Technical Instructions
* **Logic/Code:** Pivot post-level information from `raw_timescaledb` using dbt transformations. Implement logic to align with Apify metrics for comparison.
* **Naming/Paths:** Model name: `stg_timescaledb_social_posts`. Snowflake Silver layer schema.
* **Security & Access:** Access is already granted between dbt and Snowflake.

#### Definition of Ready (DoR)
- [x] Access to required systems/sources is granted
- [x] Documentation or designs are available and linked in Background
- [ ] Upstream dependencies (NXS-492) are identified and complete

#### Definition of Done (DoD)
- [x] Code follows naming conventions (`stg_timescaledb_social_posts`)
- [ ] Unit tests or dbt tests passed
- [ ] Documentation updated in .yml or Confluence
- [ ] Data integrity verified (row counts / schema match)
- [ ] Deployment completed
