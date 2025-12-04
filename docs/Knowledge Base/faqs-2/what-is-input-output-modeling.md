---
title: What Is Input-Output Modeling?
deprecated: false
hidden: false
metadata:
  robots: index
---
_**Input-Output (I-O) modeling**_ is a specialized field of economics with more than a century of history. These models are mathematically complex and traditionally explained using advanced economic concepts and applied linear algebra. ------ cross link TBD

The following provides a non-technical introduction to I-O modeling and an overview of the data sources used in the Lightcast Input-Output model.

## I-O Overview

Input-Output models describe the flow of money within an economy, focusing primarily on the financial interactions among industries. These interactions are organized within a standardized accounting structure known as input-output accounts.

A portion of one industry’s output (its sales) becomes another industry’s input (its purchases). By mapping these relationships, I-O accounts help illustrate how industries rely on one another.

In the United States, the Bureau of Economic Analysis (BEA) produces the core Industry Economic Accounts that underpin all national I-O models. These tables summarize which industries produce and consume specific commodities and in what quantities.

To make this information actionable at a local level, national tables must be **regionalized**. Regionalization adjusts the national data using each region’s unique industry composition and other relevant datasets. This process estimates

* How much of each industry’s inputs are purchased locally?
* How much of each industry’s outputs are exported?

Most modern I-O models including Lightcast’s use non-survey regionalization techniques that combine multiple regional data sources with the region’s own industry mix.

The result is a region-specific table showing the percentage of each industry’s inputs derived from every other industry. This table forms the foundation of any regional I-O model.

Lightcast’s multi-regional I-O model is a non-survey model capable of analyzing transactions and ripple effects (multipliers) across multiple regions. Regions are defined as collections of counties. When a user builds a multi-regional model, the system aggregates the relevant regional data and estimates the transactions occurring among those regions.

## Lightcast I-O Model Data Sources

To produce regionalized estimates, the Lightcast model draws on a wide array of internal and external datasets, most compiled by U.S. federal agencies. The key sources are summarized below.

### Lightcast Data

Lightcast generates detailed industry, occupation, and demographic data at the local level. This includes jobs and earnings data, which supports the regionalization of national matrices and allows the model to disaggregate industries into finer detail than federal datasets typically provide. In particular, sales-to-jobs and earnings-to-sales ratios are crucial inputs.

### BEA 

**Make and Use Tables (MUTs)**

The MUTs form the foundation of U.S. I-O modeling.

* The Make Table shows how much of each commodity is produced by each industry.
* The Use Table shows how much of each commodity is consumed by each industry.

Lightcast uses MUTs to build an industry-by-industry matrix of all industry purchases from every other industry.

**Gross Domestic Product by State (GSP)**

GSP data acts as a control within the model. Selected components of the Lightcast model are aligned (**pegged**) to values from this dataset.

**National Income and Product Accounts (NIPA)**

NIPA provides broad national economic measures. Lightcast uses these data as seeds and controls throughout multi-regional modeling.

**Local Area Income (LPI)**

LPI includes the CA05 table, which details personal income and earnings by industry. It supports place of work versus place of residence adjustments and helps estimate personal income components such as transfers, dividends, interest, and rent.

### BLS 

**Consumer Expenditure Survey (CEX)**

CEX provides insights into consumer spending patterns, income characteristics, and demographic profiles. Lightcast uses CEX extensively to build national demographic by income consumption models.

### Census Bureau 

**Census of Governments (CoG)**

The state and local finance datasets help separate government data reported in the MUTs. This allows the model to create distinct production functions for each level of government.

**LODES (Longitudinal Employer-Household Dynamics) Data**

LODES includes three datasets at the census block level

* Origin-Destination (OD) Jobs counted by home and work census blocks
* Residence Area Characteristics (RAC) Jobs counted by home census block
* Workplace Area Characteristics (WAC) Jobs counted by work census block

These datasets support the model’s commuting submodel, which estimates earnings classified as commuting income. When LODES data is unavailable for certain years or regions, gaps are filled using ACS-based commuting flows.

**Current Population Survey (CPS)**

CPS supplies demographic ratios and income distributions used to classify households into three income categories: wages, property income, and transfers.

**American Community Survey (ACS)**

County to County Commuting Flows Used to supplement LODES for years or areas where LODES data is incomplete.

**ACS Public Use Microdata Sample (PUMS)**

Serves as a supplemental source for filling gaps in CPS demographic data.

### Other Data Sources

**Oak Ridge National Laboratory (ORNL)**

County-to-County Distance Matrix, This dataset contains distance and impedance measures between county centroids via highway, rail, water, or combined routes. It also includes minimum impedance paths. Lightcast uses this in its gravitational flows model, which estimates trade flows between counties.
