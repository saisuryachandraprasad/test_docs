---
title: Occupational Employment and Wage Statistics (OEWS)
deprecated: false
hidden: false
metadata:
  robots: index
---
***The Occupational Employment and Wage Statistics (OEWS)*** program produces employment and wage estimates for most occupations   ----- cross link TBD

* **National level**: by occupation, industry, and sector
* **State** and **MSA/non-MSA levels**: by occupation

OEWS covers 1.1 million establishments and approximately 57% of U.S. employment. It includes railroad employment but excludes military, agriculture, fishing, forestry, private households, self-employment, and several other categories.

## How Lightcast Incorporates OEWS

Lightcast uses OEWS as its primary occupation data source. However, because OEWS has limitations particularly in historical continuity and coverage we strengthen it by integrating more reliable industry employment data from

* Quarterly Census of Employment and Wages (QCEW)
* County Business Patterns (CBP)
* American Community Survey (ACS)
* Other vetted sources

Lightcast applies regionalized OEWS-based staffing patterns to these industry datasets to distribute employment across occupations at detailed geographic levels.

Earnings data also comes from OEWS. Lightcast

* Uses unsuppression techniques to fill missing values when appropriate
* Builds a continuous time series to support historical occupation earnings analysis

A detailed explanation of Lightcast’s occupation methodology is available in a related ***article***. ----- cross link TBD

## Strengths 

* Provides industry-specific occupational employment and wage estimates at the national level
* Provides cross-industry occupation estimates for each state
* Includes MSA and non-MSA estimates, covering all U.S. geographic regions

## Weaknesses 

* OEWS is a survey, not an administrative dataset; it is less comprehensive than QCEW
* Not all metropolitan or nonmetropolitan areas have data for every occupation
* Covers only 57% of U.S. employment (vs. 95% of wage-and-salary jobs in QCEW)
  * Excludes most of NAICS 11 (agriculture, forestry, fishing, and hunting) except logging and certain support activities
* The survey takes up to three years to complete, limiting its usefulness for analyzing year-over-year changes
  * Apparent changes in wages or employment may reflect methodological differences, not real labor-market shifts

Lightcast’s occupational methodology is designed to account for these limitations and produce more stable and reliable historical estimates.
