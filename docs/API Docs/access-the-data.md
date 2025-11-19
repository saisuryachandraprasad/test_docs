---
title: Access the Data
deprecated: false
hidden: false
metadata:
  robots: index
---
This page helps you understand the supported methods to access our data. You can retrieve data using the API or through several cloud-based data-share delivery options. Use this guidance to select the method that best fits your workflow, integration, and storage requirements.

We provide two primary methods to access data:

* **API:** For programmatic access and real-time integration.
* **Data Shares:** For bulk storage, cloud-native analytics, and managed data delivery.

Each method offers different capabilities depending on whether you need on-demand requests, scheduled updates, or direct access through your cloud environment.

## Access Methods

### Use the API:

Use the API to retrieve data directly and integrate to your applications or products. This method is suited for **real-time queries**, **automated workflows**, or **lightweight integrations**.

Key Capabilities:

* Retrieve data on demand.
* Use filters and parameters to refine responses.
* Integrate with workflows using standard conventions.

The API is recommended when you want flexibility, rapid iteration, or granular control over your queries. You can explore our [API reference](https://docs.lightcast.io/lightcast-api/reference)  for more information

### Use Data Shares

Data Shares provide direct access to our datasets through your preferred cloud platforms or storage environments. This method is designed for teams that need **scalable access**, **recurring updates**, or **cloud-native compute capabilities**.

Supported Data Share options:

<Cards columns={4}>
  <Card title="Amazon S3 " href="https://lightcast.io/resources/blog/connecting-amazon-s3-with-lightcast-data-shares" icon="fa-user" target="_blank">
    **Provides bulk data files in a secure object-storage environment**
  </Card>

  <Card title="Databricks" icon="fa-database">
    **Allows you to query shared tables in a unified analytics workspace.**
  </Card>

  <Card title="Google BigQuery" icon="fa-user">
    **Enables SQL-based access with serverless analytics at scale.**
  </Card>

  <Card title="Google Cloud Storage" icon="fa-cloud">
    **Offers direct access to file-based datasets in your Google Cloud environment.**
  </Card>

  <Card title="Microsoft Azure Blob Storage" icon="fa-user">
    **Provides object storage for Azure-based workflows.**
  </Card>

  <Card title="SFTP" icon="fa-user">
    **Supports periodic or automated file transfers over a secure channel.**
  </Card>

  <Card title="Snowflake" icon="fa-user">
    **Provides direct warehouse access**
  </Card>

  <Card title="Snowflake Marketplace" icon="fa-user">
    **Explore our data at marketplace**
  </Card>

  <Card title="Databricks Marketplace" icon="fa-user">
    **Browse our data in marketplace**
  </Card>
</Cards>

You can find the schema definitions for our marketplace datasets [here](https://docs.lightcast.dev/data-shares) .

Choose the right method:

| Requirement                             | Recommended Methods                                                 |
| :-------------------------------------- | :------------------------------------------------------------------ |
| Programmatic, real-time access          | API                                                                 |
| Bulk or historical data delivery        | Amazon S3, Google Cloud Storage, Microsoft Azure Blob Storage, SFTP |
| Cloud-native SQL workloads              | Google BigQuery, Databricks, Snowflake                              |
| File-based ingestion from cloud storage | Amazon S3, Google Cloud Storage, Microsoft Azure Blob Storage       |
| Marketplace                             | Snowflake Marketplace, Databricks Marketplace                       |

<br />

<Cards columns={4} className="rcards">
  <Card title="Amazon S3" href="/docs/aws-s3" className="rmd-card">
    <div className="rmd-card-media" role="img" aria-label="Amazon S3 object storage">
      <img className="rmd-lazy" data-src="https://example.com/images/aws-s3-hero.jpg" alt="Amazon S3 object storage" />
    </div>

    <div className="rmd-card-body">
      <h3 className="rmd-card-title">Amazon S3</h3>
      <p className="rmd-card-desc"><strong>Bulk data files in a secure object-storage environment.</strong></p>

      <div className="rmd-card-meta">
        <span className="rmd-badge">File share</span>
        <a className="rmd-cta" href="https://lightcast.io/resources/blog/connecting-amazon-s3-with-lightcast-data-shares" target="_blank" rel="noopener noreferrer">Read more →</a>
      </div>
    </div>
  </Card>

  <Card title="Databricks" className="rmd-card">
    <div className="rmd-card-media" role="img" aria-label="Databricks">
      <img className="rmd-lazy" data-src="https://example.com/images/databricks-hero.jpg" alt="Databricks" />
    </div>

    <div className="rmd-card-body">
      <h3 className="rmd-card-title">Databricks</h3>
      <p className="rmd-card-desc"><strong>Query shared tables inside a unified analytics workspace.</strong></p>

      <div className="rmd-card-meta">
        <span className="rmd-badge">Query</span>
        <a className="rmd-cta" href="/docs/databricks-integration">Learn →</a>
      </div>
    </div>
  </Card>

  <Card title="Google BigQuery" className="rmd-card">
    <div className="rmd-card-media" role="img" aria-label="Google BigQuery">
      <img className="rmd-lazy" data-src="https://example.com/images/bigquery-hero.jpg" alt="Google BigQuery" />
    </div>

    <div className="rmd-card-body">
      <h3 className="rmd-card-title">Google BigQuery</h3>
      <p className="rmd-card-desc"><strong>SQL access with serverless analytics at scale.</strong></p>

      <div className="rmd-card-meta">
        <span className="rmd-badge">SQL</span>
        <a className="rmd-cta" href="/docs/bigquery">Docs →</a>
      </div>
    </div>
  </Card>

  <Card title="Google Cloud Storage" className="rmd-card">
    <div className="rmd-card-media" role="img" aria-label="Google Cloud Storage">
      <img className="rmd-lazy" data-src="https://example.com/images/gcs-hero.jpg" alt="Google Cloud Storage" />
    </div>

    <div className="rmd-card-body">
      <h3 className="rmd-card-title">Google Cloud Storage</h3>
      <p className="rmd-card-desc"><strong>Direct access to file-based datasets in Google Cloud.</strong></p>

      <div className="rmd-card-meta">
        <span className="rmd-badge">File</span>
        <a className="rmd-cta" href="/docs/gcs">Docs →</a>
      </div>
    </div>
  </Card>
</Cards>
