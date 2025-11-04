---
title: Canada Industry
deprecated: false
hidden: false
metadata:
  robots: index
---
## Introduction

The Canada Industry dataset provides essential insights into Canadian labor market, offering both historical and projected data on industry employment and earnings. It enables users to analyze workforce trends, evaluate economic performance, and compare industries across regions and time period. It covers historical data since 2001 to current industry year and project data for current industry year.

> Current Industry Year refers to most recent year. This may differ from calendar year.

## Popular Use Cases

## Metrics

* jobs: Total number of occupied positions.
* Earnings: Total earnings for the industry since 2001 to current year.
* EPW: Earnings per worker since 2001 to current year / Total number of occupied positions.

<br />

## Filters

you can use following dimensions to filter dataset.

* Class of Worker
* Area (Hierarchy: Nation, Province, Census Division, and Census Sub-division)
* Industry (2 to 4 digits <Anchor label="NAICS" target="_blank" href="https://kb.lightcast.io/en/articles/7934064-north-american-industry-classification-system-naics">NAICS</Anchor>)
* Year

## Metadata

* Access
* Dataset ID
* Dataset URL
* Format
* Data size
* Update frequency
* Versions
* Metrics
* Dimensions
* Attributes

<br />

## Schema

<br />

| Fields       | Snowflake | BigQuery   | Databricks | Description                                                                                                                                    |
| :----------- | :-------- | :--------- | :--------- | :--------------------------------------------------------------------------------------------------------------------------------------------- |
| AREAID       | VARCHAR   | STRING     | STRING     | ID of the geographic region.                                                                                                                   |
| AREAID_NAME  | VARCHAR   | STRING     | STRING     | Name of the geographic region.                                                                                                                 |
| AREAID_TYPE  | VARCHAR   | STRING     | STRING     | Geographic area type.                                                                                                                          |
| CLASSID      | VARCHAR   | STRING     | STRING     | ID of the class of worker.                                                                                                                     |
| CLASSID_NAME | VARCHAR   | STRING     | STRING     | Name of the class of worker.                                                                                                                   |
| EARN         | FLOAT     | FLOAT      | DOUBLE     | Total earnings for the industry (wages + supplements). This figure is also for the whole industry, not for the average worker in the industry. |
| EMP          | FLOAT     | FLOAT      | DOUBLE     | The number of occupied positions.                                                                                                              |
| INDID        | VARCHAR   | STRING     | STRING     | NAICS code.                                                                                                                                    |
| INDID_NAME   | VARCHAR   | STRING     | STRING     | NAICS name.                                                                                                                                    |
| YEAR         | NUMBER    | BIGNUMERIC | DECIMAL    | Year of data.                                                                                                                                  |

<br />

<br />
