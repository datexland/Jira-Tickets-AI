#### Title  

> Installing Python Dependencies via plugins.zip

#### Description
As a Data Engineer, I want to install the `apache-airflow-providers-dbt-cloud==4.4.2` dependency via a `plugins.zip` file, So that we can run dbt jobs from our MWAA Airflow environment which is currently restricted within a private network.

#### Background

The MWAA environment is hosted within a private network without public internet access, preventing the automatic download of Python packages during environment startup. To enable dbt job execution, the required provider must be manually bundled and provided to the environment. This task involves creating and configuring the `plugins.zip` package to include the necessary dbt-cloud provider.

#### Technical Instructions
* **Component A – Logic/Code:** Package the `apache-airflow-providers-dbt-cloud==4.4.2` library into a `plugins.zip` file compatible with the MWAA Airflow version.
* **Component B – Naming/Paths:** The final file must be named `plugins.zip`. (Ensure it is uploaded to the designated S3 bucket path configured for the MWAA environment).
* **Security & Access:** N/A - Standard deployment permissions to S3 and MWAA console required.

#### Definition of Ready (DoR)
- [x] Access to required systems/sources (S3/MWAA) is granted
- [x] Documentation or designs are available and linked in Background
- [x] Upstream dependencies (ticket numbers) are identified and complete
*(Agent Note: Check off completed items based on user conversation)*

#### Definition of Done (DoD)
- [ ] Code follows naming conventions (e.g., `plugins.zip`)
- [ ] Unit tests or dbt tests passed (verified by successful DAG import in MWAA)
- [ ] Deployment completed and observability verified in MWAA logs
