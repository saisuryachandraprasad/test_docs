---
title: 'Lightcast SOC  '
excerpt: >-
  This article explains how Lightcast SOC codes differ from the standard SOC
  system and the reasons for those differences.rences.
deprecated: false
hidden: false
metadata:
  robots: index
---
## SOC 2021

Lightcast follows the Standard Occupation Classification (SOC) structure used in the Occupational Employment and Wage Statistics (OEWS) program, which is Lightcast's primary source of occupation data. As of Spring 2022, OEWS uses SOC 2018.

Because of the deviations described below, Lightcast refers to its internal version as SOC 2021, corresponding to the first OEWS data release in which these codes appeared. The taxonomy remains aligned with the 2018 SOC System.

## SOC Particularities

Lightcast generally adopts the SOC conventions used in OEWS. However, several important exceptions apply, driven by data availability and reporting practices.

Key Differences

**Military Occupations**

Lightcast does not use detailed SOC military codes due to limited data quality. Instead, Lightcast aggregates all 20 military occupations into a single code: 55-9999.

**Postsecondary Teachers**

Lightcast uses a single aggregated code 25-1099 for all postsecondary teachers, replacing the 38 detailed SOC codes.
This decision is based on insufficiently reliable data. 

> Lightcast research on this topic is available here. -------cross link TBD

**Unclassified Occupations**

Lightcast adds 99-9999 (Unclassified Occupation) for Extended Proprietors in industries where occupational estimates cannot be produced reliably.

**Substitute Teachers**

Following OEWS, Lightcast includes 25-3098 (Substitute Teachers).

**O_NET Codes Without Tasks**

Lightcast excludes O_NET codes lacking assigned task statements, which generally correspond to All Other catchall categories.

## Additional Reasons 

Beyond the exceptions above, Lightcast SOC codes may differ from other published SOC sources due to the following

**Alignment with OEWS**

OEWS occasionally uses classifications that differ slightly from the official SOC 2018 system. Lightcast conforms to OEWS for consistency with its primary data source.

**Clarifying Broad** vs. **Detailed Codes**

When OEWS reports a broad code and a detailed code with identical numeric values, Lightcast changes the detailed code’s ending from -XXX0 to -XXX8. This avoids confusion between hierarchy levels.

*Examples of Lightcast SOC differences*

| **Lightcast SOC** | **Lightcast SOC Name**                                                                               | **OEWS SOC** | **Notes on Lightcast change**                                                 |
| ----------------- | ---------------------------------------------------------------------------------------------------- | ------------ | ----------------------------------------------------------------------------- |
| 13-1028           | Buyers and Purchasing Agents                                                                         | 13-1020      | Code changed from XXX0 to XXX8                                                |
| 13-2028           | Property Appraisers and Assessors                                                                    | 13-2020      | Code changed from XXX0 to XXX8                                                |
| 21-1018           | Substance Abuse, Behavioral Disorder, and Mental Health Counselors                                   | 21-1018      | follows OEWS change                                                           |
| 25-1099           | Postsecondary Teachers                                                                               | (see above)  |                                                                               |
| 25-2052           | Special Education Teachers, Kindergarten and Elementary School                                       | 25-2052      | Combines Standard SOC 25-2055 and 25-2056                                     |
| 25-9045           | Teaching Assistants, Except Postsecondary                                                            | 25-9045      | Combines Standard SOC 25-9042 and 25-9043                                     |
| 29-2018           | Clinical Laboratory Technologists and Technicians                                                    | 20-2010      | Code changed from XXX0 to XXX8                                                |
| 31-1128           | Home Health and Personal Care Aides                                                                  | 31-1120      | Code changed from XXX0 to XXX8                                                |
| 39-7018           | Tour and Travel Guides                                                                               | 39-7010      | Code changed from XXX0 to XXX8                                                |
| 47-4098           | Miscellaneous Construction and Related Workers                                                       | 47-4090      | Code changed from -XXX0 to -XXX8                                              |
| 51-2028           | Electrical, Electronic, and Electromechanical Assemblers, Except Coil Winders, Tapers, and Finishers | 51-2028      | Code changed from -XXX0 to -XXX8                                              |
| 51-2098           | Miscellaneous Assemblers and Fabricators                                                             | 51-2090      | Code changed from -XXX0 to -XXX8                                              |
| 53-1047           | First-Line Supervisors of Transportation and Material Moving Workers, Except Aircraft Cargo Handling | 53-1047      | Combines standard SOC 53-1042, 53-1043, 53-1044, and 53-1049 to form this SOC |
| 55-9999           | Military-only occupations                                                                            | (see above)  |                                                                               |
| 99-9999           | Unclassified Occupation                                                                              | (see above)  |                                                                               |

<br />
