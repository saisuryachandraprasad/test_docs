---
title: Labor Force Participation Rate
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

The Labor Force Participation Rate (LFPR) measures the share of the population that is active in the labor market either employed or actively searching for work. It is calculated as

`LFPR = (Employed Population + Unemployed Population) / Total Civilian Non-Institutionalized Population`

The denominator excludes individuals outside the civilian, non-institutionalized population because the goal is to compare labor-force activity only among those reasonably expected to participate in the labor pool.

Traditional BLS/DOL definition: Civilian non-institutionalized population ages 16 and older.

## Sources and Methodology

### Employment and Unemployment

Lightcast sources employment and unemployment counts directly from the Bureau of Labor Statistics’ Local Area Unemployment Statistics (LAUS) program. This data is not modeled by Lightcast; we use LAUS ***definitions***, including ------ cross link TBD

`The labor force = civilian non-institutional population ages 16+ classified as employed or unemployed`

### Population Denominator

The population denominator is derived from Lightcast’s proprietary population demographics dataset, primarily sourced from the Census Bureau’s Population and Housing Estimates (POPEST) program. POPEST represents the total resident population.

Because the LFPR denominator must reflect the civilian non-institutionalized population, Lightcast applies ratios from the American Community Survey (ACS) 5-year estimates to remove institutionalized and non-civilian populations from the POPEST counts.

### Data Quality Considerations

Modeled LAUS data can contain anomalies that result in LFPR values at or above 100%. For example, Loving County, TX has a resident population of roughly 200 (POPEST), yet LAUS reports a labor force of approximately 300 an impossible scenario that reflects low-quality inputs rather than a true labor-market condition.
