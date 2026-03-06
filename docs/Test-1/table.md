---
title: Table
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

| Column Name  | Snowflake | Big Query  | Databricks | Parquet | Comment                                                                 |
| :----------- | :-------- | :--------- | :--------- | :------ | :---------------------------------------------------------------------- |
| INDID        | VARCHAR   | STRING     | STRING     | STRING  | NACE code (taxonomy version: see CORELMI_GLOBAL_DETAILED.CORELMI_META). |
| INDID_PARENT | VARCHAR   | STRING     | STRING     | STRING  | Parent of the NACE code (in hierarchy).                                 |
| LEVEL        | NUMBER    | BIGNUMERIC | DECIMAL    | DECIMAL | Level of the dimension hierarchy.                                       |
| NAME         | VARCHAR   | STRING     | STRING     | STRING  | Industry Dimension Name                                                 |
