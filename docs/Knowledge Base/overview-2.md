---
title: Overview
deprecated: false
hidden: false
metadata:
  robots: index
---
Lightcast brings together a wide range of labor market information in one place. This includes economic, workforce, demographic, education, profile, and job posting data. The data is gathered from trusted public and private sources and is available at multiple levels-national, state, metro, county, and ZIP code.

> _**Check out**_ list of sources for Lightcast's data --- Cross link TBD

**How Often the Data Is Updated**

|               |                                                                                                                                                                                                               |
| :------------ | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Core LMI Data | Industry, occupation, education, and demographic information is updated **every quarter**. Each new **datarun** includes the latest available data from all our sources and is released early in the quarter. |
| Job Postings  | Job postings are collected and refreshed **every day**. Monthly posting totals are finalized a few days after the **month ends**.                                                                             |
| Profiles      | New and updated workforce profiles are added **each quarter**. Additional improvements-such as enhanced tagging for skills, employers, and occupations-are released every four weeks.                         |

## Job Postings

Lightcast gathers job postings from more than 220,000 sources worldwide, including company career sites, job boards, and aggregators.

**Removing Duplicate Job Posts**

To ensure accuracy, Lightcast uses a two-step process that removes up to 80% of duplicate postings

* **Within a single website**: The system checks whether a posting is truly new for that source and avoids collecting older copies.
* **Across multiple websites**: The system compares fields such as job title, employer, and location over the past 60 days. If the same job appears on different sites, it’s counted once.

<Accordion title="Example" icon="fa-info-wheel">
  If a company posts a new **Marketing Specialist** role on March 1, we treat that version as the original. Any matching versions found for the next 60 days are considered duplicates-even if the job appears daily across many job boards.
</Accordion>

**Enrichment**

Each posting is enhanced with standardized job titles, employer names, skills, SOC/NAICS codes, and details on required education and experience.

> You can refer _**Job Postings Analytics**_ process for detailed explanation

## Profiles

Lightcast maintains a large database of worker profiles—more than 100 million individuals. These profiles come from:

* Publicly available online information
* Resume databases and job boards
* Recruiting and employer systems
* CRM and marketing databases
* Consumer and identity data sources

We remove duplicate profiles with the help of Machine Learning algorithms and standardize titles, skills, employers, and education details. This makes the data more reliable and easier to understand.

> You can get more detailed explanation on profile methodology _**here**_ --- cross link TBD

## Industries

Industry data describes jobs and wages based on the type of business, such as healthcare, manufacturing, or retail.

**Key Sources**

* The Quarterly Census of Employment and Wages (QCEW) from the Bureau of Labor Statistics, which covers about 95% of U.S. employment.
* The Census County Business Patterns (CBP) dataset, which fills gaps where QCEW suppresses data.
* The American Community Survey (ACS), which adds information about self-employed workers.
* Data is available back to 2001.

**Projections**

ABC builds 10-year industry projections by analyzing historical trends and adjusting them using national and state forecasts. Industry earnings data is not projected.

> Refer _**Industry Projections Methodology**_ for detailed explanation --- Link TBD

## Occupations

Occupation data shows employment and wages for specific types of workers, such as Registered Nurses or Web Developers, Welders, etc.

**How Lightcast Builds Occupation Data**

* Industry job counts from Quarterly Census of Employment and Wages (QCEW)
* Staffing patterns from the Occupational Employment and Wage Statistics (OEWS) dataset
* Local adjustments based on regional industry mix

Lightcast also creates a historical wage time series back to 2005 to reduce year-to-year variability.

**Title and Skill Level Estimates**

Lightcast uses a compensation model that blends occupation-level wage data with more detailed worker profile information to estimate earnings for specific job titles and skills.

> Refer _**Compensation Model for detailed explanation**_ -- Cross link TBD

**Projections**: Occupation employment data is projected 10 years forward using projected industry trends. Earnings are not projected.

## Education

Lightcast uses the IPEDS dataset from the National Center for Education Statistics (NCES) to report on college enrollments, graduates, tuition, and completions. Data includes gender and race/ethnicity details.

IPEDS releases updates throughout the year, and we incorporate them as they become available. Most new completions data arrives in late summer.

## Demographics

Most demographic information comes from the Census Bureau’s Population Estimates Program. Data covers age, gender, and race/ethnicity at the county level.

**To create ZIP-code estimates**:

* Models Census Tract data using the ACS
* Uses Housing and Urban Development (HUD) mapping tools to convert tract-level estimates into ZIP-code values

Lightcast also projects demographic trends 10 years into the future using a cohort model.
