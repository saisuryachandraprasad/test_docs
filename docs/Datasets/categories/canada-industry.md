---
title: Canada Industry
deprecated: false
hidden: false
metadata:
  robots: index
---
## Metadata

You can access this dataset via [Core LMI API](https://docs.lightcast.io/lightcast-api/reference/overview-core-lmi)  

<br />

## Schema

<br />

| Field       | AREAID                       | AREAID_NAME                    | AREAID_TYPE           | CLASSID                    | CLASSID_NAME                 | EARN                                                      | EMP                          | INDID       | INDID_NAME  | YEAR         |
| :---------- | :--------------------------- | :----------------------------- | :-------------------- | :------------------------- | :--------------------------- | :-------------------------------------------------------- | :--------------------------- | :---------- | :---------- | :----------- |
| Description | ID of the geographic region. | Name of the geographic region. | Geographic area type. | ID of the class of worker. | Name of the class of worker. | Total earnings for the industry (wages + supplements).    | Number of occupied positions | NAICS Code  | NAICS Name  | Year of Data |
| Snowflake   | VARCHAR                      | VARCHAR                        | VARCHAR               | VARCHAR                    | VARCHAR                      | Float                                                     | Float                        | VARCHAR     | VARCHAR     | Number       |
| BigQuery    | STRING                       | STRING                         | STRING                | STRING                     | STRING                       | Float                                                     | Float                        | STRING      | STRING      | Big Numeric  |
| Databricks  | STRING                       | STRING                         | STRING                | STRING                     | STRING                       | Double                                                    | Double                       | STRING      | STRING      | Decimal      |

<br />

<br />
