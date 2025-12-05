---
title: Quarterly Census of Employment and Wages (QCEW)
deprecated: false
hidden: false
metadata:
  robots: index
---
The Quarterly Census of Employment and Wages (QCEW) is a dataset published by the U.S. Bureau of Labor Statistics (BLS). QCEW forms the backbone of Lightcast’s core labor market data, providing establishment counts, monthly employment, and quarterly wages by

* NAICS industry
* County
* Ownership sector

These data cover the entire United States and are aggregated to

* Annual levels
* Higher industry groupings (industry groups, sectors, supersectors)
* Higher geographic levels (***MSA***, state, national) ------ cross link TBD

**Enhancements to QCEW**

Lightcast produces a slightly modified version of the original BLS QCEW dataset to improve completeness and consistency

* Unsuppression of data Lightcast estimates values for suppressed cells (approximately 60% of QCEW data).
* Adjusted NAICS classifications for public-sector employment Updated to improve compatibility with other Lightcast data sources.
* Standardized county and NAICS definitions Lightcast apply consistent definitions from 2001 forward BLS QCEW does not maintain consistent year-to-year definitions.

> You can explore suppression and NAICS for detailed explanation.

**Strengths**

* **High reliability**: QCEW is based on official employer records collected through state and federal unemployment insurance programs and is widely considered the gold standard for industry employment data in the U.S.
* **Comprehensive coverage**: QCEW captures approximately 95% of all U.S. wage and salary jobs.
* **Flexible granularity**: Data are available at multiple geographic levels (county, MSA, state, national) and at detailed NAICS levels (2–6 digit).

**Weaknesses**

* **Data lag**: There is typically a five- to six-month delay between data collection and public release; updates occur quarterly.
* **High suppression rate**: Roughly 60% of private-sector county-level data is suppressed to protect employer confidentiality.

Limited coverage of certain worker types QCEW does not include

* Self-employed workers
* Military personnel
* Railroad workers
* Many agricultural, domestic, and nonprofit workers
