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
