---
title: Workforce Estimation Model (WEMo)
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Lightcast estimates workforce size by region and occupation within the Global dataset, available in Talent Analyst and through the API. These estimates are produced using the proprietary **Workforce Estimation Model** (WEMo).

WEMo integrates multiple _**government data**_ sources and labor market patterns derived from ***job postings** to generate detailed, globally comparable talent pool estimates.     ----- cross link TBD

Global labor market data presents several challenges due to differences in

* Language
* Data availability
* Update cadences
* Job categories and definitions
* Regional boundaries and classification systems

WEMo applies standardized methodologies and taxonomies to address these challenges and ensure consistency across countries. A full list of supported countries is available in the Available _**Countries in Global table**_. ----- cross link TBD

## Data Sources

WEMo relies primarily on government workforce datasets, supplemented with job postings data.

**Government Workforce Data**

Lightcast collects workforce information from local government agencies and international organizations. Each dataset is evaluated for

* **Coverage**: Whether it reflects the full economy
* **Recency**: How recently the data was collected
* **Methodology**: Sample size, modeling practices, and reporting standards

Details on the specific workforce sources used for each country are available in the _**country methodology table**_. ------- cross link TBD

**Job Postings Data**

Lightcast collects job postings daily from a wide range of global sources, including

* Applicant tracking systems
* Employer job boards
* High-quality secondary aggregators

All postings are translated and classified to enable consistent cross-country analysis. After collection, government data and job postings are mapped to shared classification systems, including

* International Standard Classification of Occupations (ISCO)
* Lightcast Occupation Taxonomy (LOT)
* Lightcast Administrative Areas (LAA)

## Methodology

The following steps describe how WEMo produces workforce estimates. Note that this process excludes the creation of LOT and LAA themselves, although both are essential to WEMo.

**Step 1**: **Standardizing Local Taxonomies**

Lightcast begins by collecting the most reliable workforce data available for each country. To compare data internationally, Lightcast builds internal crosswalks that map local job taxonomies to the ISCO structure. This ensures consistency across countries.

ISCO provides broad global occupational categories approximately **400+** which is less granular than other taxonomies such as,

* U.S. SOC (800+ categories)
* Lightcast LOT (1,900+ categories)

**Step 2**: **Modeling ISCO to LOT Granularity**

After aligning local data with ISCO, WEMo models ISCO categories down to the more granular LOT taxonomy. This is achieved by applying job posting based distribution patterns that are specific to each country.

**Step 3**: **Creating Ratio Distributions**

Each LOT Specialized Occupation is linked to a corresponding 4-digit ISCO occupation. Using three years of region-specific job postings classified by LOT Specialized Occupation, Lightcast calculates ratio distributions that describe how each LOT role is represented within its ISCO group in that region.

**Step 4**: **Estimating Workforce Size**

Lightcast applies these ratios to the government workforce data to estimate employment counts for each LOT occupation. Results are expressed as a range (low, middle, high) to reflect the confidence level.

_Example_: Estimated Java Developers in Germany

* Low: 27,018
* Middle: 29,947
* High: 32,876

In essence, WEMo combines government data with data-driven distribution patterns from job postings to model workforce size by region and occupation.

## Confidence Levels

WEMo presents results as a range to reflect uncertainty. Confidence levels depend on

* Data volume
* Data recency
* Market stability

ABC calculates confidence using the following formula `distance = (high – mid) / mid`

The distance value determines the confidence level

| Level | Distance Range | Confidence Term     |
| :---- | :------------- | :------------------ |
| 5     | \< 0.061       | Extreme confidence  |
| 4     | 0.061–0.137    | High confidence     |
| 3     | 0.136–0.226    | Moderate confidence |
| 2     | 0.225–0.363    | Marginal confidence |
| 1     | > 0.363        | Minimal confidence  |

WEMo is designed not to generate estimates where input data is insufficient or unreliable. Some countries therefore do not produce WEMo results. A complete list of supported countries is provided in the Available Countries in Global table.
