---
title: US - United States Methodology
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Lightcast uses labor market data to connect and inform individuals, educational institutions, and employers. To support this mission, Lightcast integrates economic, labor market, demographic, and education data from dozens of government and private-sector sources. The result is a comprehensive and current database that includes officially published data as well as detailed estimates with full U.S. coverage.

With Lightcast Global, data from multiple countries is aligned across geographies into an international dataset. Because each nation collects and publishes data differently, this harmonization process can reduce some granularity. For highly detailed U.S. information such as granular skills, compensation insights, or ZIP-level employment Lightcast recommends using the _**Analyst**_ tool. ---- cross link TBD

<Callout icon="⚙️" theme="default">
  In addition to the LMI sources described here, Lightcast also provides insights through _**Global Postings**_ and _**Global Worker Profiles**_ in the United States.   ---- cross link TBD
</Callout>

## Lightcast Data Sources

Lightcast draws from a wide range of federal datasets. Key sources include

<Accordion title="Bureau of Labor Statistics (BLS)">
  * Current Employment Statistics (CES)
  * Local Area Unemployment Statistics (LAUS)
  * National Employment Projections
  * Occupational Employment Statistics (OES)
  * Quarterly Census of Employment and Wages (QCEW)
  * National Industry Occupation Employment Matrix (NIOEM)
  * Occupational Education and Training Projections
</Accordion>

<Accordion title="Census Bureau">
  * American Community Survey (ACS)
  * County Business Patterns (CBP)
  * Current Population Survey (CPS)
  * Non-Employer Statistics (NES)
  * Quarterly Workforce Indicators (QWI)
  * TIGER/Line Map Files
  * ZIP Code Business Patterns (ZBP)
  * LEHD Origin–Destination Employment Statistics (LODES)
  * Population Estimates
  * National and State Population Projections
  * Census 2000 & 2010 Summary Files
  * Census of State & Local Governments
</Accordion>

<Accordion title="Department of Labor, Employment and Training Administration">
  * Characteristics of the Insured Unemployed (CIU)
  * O\*NET Database
</Accordion>

## Occupation Data

U.S. occupation data is generally less complete and less reliable than industry data. As a result, Lightcast builds occupation estimates by applying staffing patterns to industry data. Staffing patterns reflect the occupational composition of each industry.

The primary sources for Lightcast staffing patterns are

* BLS Occupational Employment Statistics (OES)
* Census American Community Survey (ACS)

**Creating Staffing Patterns for QCEW/Non-QCEW Employee Jobs**

Lightcast produces staffing patterns for employee jobs through the following process:

1. Obtain the most recent OES staffing pattern and OES metro-level occupation data, then unsuppress both datasets.
2. Use metro-level QCEW industry data (aligned with OES coverage), the national OES staffing pattern, and OES metro occupation totals to regionalize the national pattern adjusting the percentages to reflect local conditions.
3. Add staffing patterns derived from ACS microdata for industries not covered by OES.

Because OES, ACS, and NIOEM differ in definitions and coverage, the resulting Lightcast national staffing pattern will differ from any single source.

### Historical Staffing Patterns

* Staffing patterns for prior years are created by back-chaining, meaning each year’s pattern is derived from the following year’s version.
* The latest staffing pattern serves as the base and is not adjusted to match earlier years.
* Due to structural changes in OES, Lightcast does not use OES data before 2005; staffing patterns for 2001–2004 are created by back-projecting the 2005 pattern.

**Creating Staffing Patterns for Self-Employed Workers**

For the self-employed, Lightcast creates a national staffing pattern using ACS microdata.

* Certain aggregated occupations are broken into more detailed categories using ratios from OES.
* This national pattern is applied to all counties due to limited geographic detail for self-employment.
* ACS-based staffing patterns are back-projected from 2004 to 2001 and forward-projected to Lightcast’s standard projection year (typically 10 years ahead).

## Occupation Classification

U.S. occupation data is classified using the Standard Occupational Classification (SOC) system. Like NAICS, SOC is hierarchical and uses hyphenated six-digit codes to divide occupations into

* Major Groups
* Minor Groups
* Broad Occupations
* Detailed Occupations

Lightcast maps SOC codes to _**Global Occupations**_ to support international consistency.   --- cross link TBD

O*NET, maintained by the U.S. Department of Labor, builds on the SOC system by adding

* Additional occupational detail
* Information on knowledge, skills, and abilities (KSAs)
* Typical education and training requirements

<br />
