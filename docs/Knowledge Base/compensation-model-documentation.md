---
title: Compensation Model Documentation
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Lightcast compensation model provides occupational wage estimates enhanced with skill and certification specific premiums. It integrates percentile wage data derived from Lightcast's labor market information (LMI) government sources with salary observations extracted from online job postings.

## Sources

The compensation model draws from two primary data sources

**Occupational Employment Statistics (OES)**

The foundation of Lightcast's occupational wage estimates is the U.S. Bureau of Labor Statistics’ Occupational Employment Statistics (OES) dataset. Updated annually, OES provides percentile wage data for occupations at the metropolitan level across the United States. When OES suppresses percentile estimates for confidentiality, Lightcast applies internal methods to unsuppress the data.

**Job Postings**

Job postings provide wage observations that can be linked directly to skills and certifications granularity not available in OES. Postings are collected from online sources and processed through Lightcast's job posting pipeline. 

> You can refere Job Postings for more detailed explanation. ---- cross link TBD

## Updates

* OES data is released annually each May.
* Job postings data is refreshed monthly.

The Lightcast compensation model is updated monthly to incorporate the most recent quarter of salary information observed in job postings.

## Process Overview

The compensation model delivers wage estimates for occupations based on the presence of specific skills or keywords.

* When an occupation is requested without skills or keyword filters, the model returns standard OES-based wage estimates, with no job posting data applied.
* When an occupation is requested with skills or keyword filters (for example, *a welder requiring GMAW and FCAW skills*), the model creates a wage curve by blending OES percentile data with wage observations from job postings that match the criteria.

A minimum of 100 matching postings is required to produce a valid sample. If fewer than 100 exist, the user is notified that no reliable estimate can be generated.

**Creation of Base National Wage Curves**

A base national wage curve is created for each occupation. This curve serves as the starting point for all user-generated wage estimates.

OES provides wage estimates at the 10th, 25th, 50th, 75th, and 90th percentiles. Lightcast then aligns wage observations from job postings each associated with various skills or keywords to the appropriate percentile ranges on the curve.

Because posting observations rarely distribute evenly across percentile bands, Lightcast applies poststratification weighting

* Ranges with fewer observations receive higher weights.
* Ranges with more observations receive lower weights.

This weighting process corrects for uneven sample distribution and produces a more stable and representative wage curve.

**Processing User Requests**

When the model receives a request

* Map job titles to SOC codes (when applicable).
* Build a national wage curve based on job postings that match the requested skills or keywords.

*Example*: if a user requests welders with GMAW and FCAW skills, the model identifies all relevant postings along the existing welder base curve and uses those with the required skills to construct a specialized curve. The sample must include at least 100 postings to be valid.

Return the specialized wage curve built from both OES percentile data and posting-based wage observations.

**Regional Estimates**

If the user requests a regional wage estimate, Lightcast applies OES based wage ratios to adjust the national curve

* National and regional OES wage curves are compared to derive the ratio.
* This ratio is then applied to the national percentiles (10th through 90th) to estimate regional wages.
* Location is not used to filter postings due to the sample-size requirement.

When a regional estimate includes skills or keywords, the model first produces the national skill-specific curve, then applies the regional ratio to generate regionalized percentiles.

**Minimum Wage Adjustment**

Due to lagging government data, some OES-based results especially at the 10th percentile may appear lower than a state’s current minimum wage. OES data reflects a three-year rolling survey and is published with an additional year of delay. Posting-based observations incorporated into the model may date back several years as well.

To ensure wage estimates remain realistic, Lightcast applies state minimum wage floors based on the minimum wage laws in effect during the most recent OES earnings year used in the model.

*Example*: For Lightcast's 2019.1 data run, the most recent OES earnings year was 2017. Therefore, the compensation model used 2017 minimum wage levels as the floor for wage estimates.
