---
title: ZIP-Level Employment Data
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Lightcast provides employment estimates by industry and occupation at the ZIP code level. These estimates begin with Lightcast’s finalized county level industry data. ZIP-level industry data is produced by disaggregating county-level industry totals using several external data sources. ZIP-level occupation estimates are then created by applying staffing patterns to the ZIP-level industry data.

Because ZIP-level data comes with specific limitations, users should review the cautions outlined later in this document.

## Creation of ZIP-Level Data

This section explains the creation of ZIP-level industry estimates, followed by the creation of ZIP-level occupation estimates.

### Modeling Industry Data from County to ZIP

Lightcast’s ZIP-level data is anchored to county-level employment figures based on the Bureau of Labor Statistics (BLS) Quarterly Census of Employment and Wages (QCEW), the most complete and reliable employment dataset in the U.S. This ensures ZIP-level estimates always aggregate exactly to county totals.

**Step 1: Distributing County Employment Using DBUSA**

DBUSA business listings provide ZIP- and industry-level employment proportions within each county.

*Example*: If a county contains three ZIP codes and has 200 jobs in Industry X, and ***DBUSA*** shows ZIP-level ratios of 57%, 43%, and 0%, Lightcast allocates 114, 85, and 0 jobs respectively. --- cross link DBUSA TBD

**Step 2: Rolling Up to Higher NAICS Levels if Needed**

If an industry exists in Lightcast’s county-level data but DBUSA shows no employment for that industry, the model checks DBUSA at higher NAICS levels (up to the 2-digit level) until data is found.

**Step 3: Fallback Using USPS DelStat Data**

If no DBUSA data is available for a county-industry combination, Lightcast uses the USPS DelStat dataset. DelStat provides business address counts by ZIP, enabling a fallback proportion based on each ZIP’s share of business addresses within the county. This fallback is used in only 0.5% of cases.

**Step 4: Producing Seed Values and Applying Unsuppression**

The percentages above produce initial seed estimates of ZIP-level employment. Lightcast’s unsuppression algorithms then adjust these values so that ZIP totals align with county-level employment. For workers covered by unemployment insurance (**class of worker 1**), the model incorporates LODES ZIP-level data to ground the adjustments in observed ZIP-level labor patterns.

Unsuppression at ZIP, tract, and city levels is performed simultaneously to ensure internal consistency across all sub-county datasets.

## Modeling ZIP Occupation Data

ZIP-level occupation estimates are created using the same methodology as Lightcast’s county-level occupation data.

1. Staffing patterns originate from the BLS Occupational Employment Statistics (OES) dataset.
2. Lightcast regionalizes these staffing patterns using regional industry and occupation data for each OES substate region.
3. The regionalized staffing patterns are applied to:
   1. County-level industry data -> County occupation estimates
   2. ZIP-level industry data -> ZIP occupation estimates

## Cautions 

Users should consider several important limitations when working with ZIP-level employment data.

**ZIP Codes Are Not True Geographies**

ZIP codes are mail delivery routes, not geographically defined areas. Many ZIP codes represent

* A single building
* A business
* A Post Office location
* A non-fixed **floating** ZIP code

Different institutions (e.g., Census Bureau, HUD) maintain their own ZIP-like definitions, updated on different schedules. As a result

* ZIP definitions vary significantly across datasets
* ZIP-based maps and visualizations often differ depending on the underlying source

> Click here to know more about floating Zip-Code    -------- cross link TBD

**USPS Monthly ZIP Updates**

USPS revises ZIP code definitions monthly as carrier routes evolve. Lightcast uses the latest USPS definition available at each quarterly data run. Many other datasets use ZIP definitions from older or non-USPS sources, which may not align with the ZIP definitions used in Lightcast data.

**Complete ZIP-Level Data Does Not Exist**

Because ZIP codes are not official geographic units, no fully comprehensive ZIP-level dataset exists.

*Examples*: Census LEHD LODES provides ZIP-level data, but only for 2-digit NAICS.

* Census ZIP Code Business Patterns (ZBP) is the most complete ZIP-level dataset available but still contains substantial gaps.

**ZIP Data Is Not a Time Series**

Lightcast ZIP data should be treated as annual snapshots, not a time series. Why because

* County-level time-series data is broken out to ZIPs using current DBUSA proportions.
* When DBUSA updates, those proportions change.
* Therefore, ZIP-level employment for all years changes with each annual update.

Because DBUSA is volatile, some ZIP-level employment fluctuations between data runs are expected.
