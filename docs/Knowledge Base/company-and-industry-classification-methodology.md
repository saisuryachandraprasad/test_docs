---
title: Company and Industry Classification Methodology
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Lightcast’s company classification system is built from more than 400 open-source company datasets, creating a comprehensive global view of employers. The system is designed to scale internationally and adapt to evolving customer needs.

* **Global Coverage**: The company classifier supports job postings and profiles from all countries for which Lightcast has data.
* **Recency**: The Lightcast Companies Taxonomy is updated monthly to reflect ongoing changes in the market.
* **Adaptability**: New metadata fields can be added to the taxonomy to meet customer-specific requirements as they evolve.

## Company Taxonomy

Lightcast maintains a global company taxonomy, refreshed monthly. Because the dataset spans a large volume of records, duplicate entries can occur. Lightcast proactively manages these records and will perform targeted cleanup or merging at customer request, in addition to our ongoing maintenance.

## How It Works

### Normalization of Raw Names

The process begins with raw company names extracted from postings and profiles. These names are normalized using proprietary rules that remove non-essential elements (such as **LLC** or **Inc**.). The result is a standardized name suitable for matching against the Lightcast Companies Taxonomy.

### Matching to Taxonomy

After normalization, each company is matched to the closest record in the taxonomy. Each company entry includes metadata such as

* Tradestyle
* NAICS codes
* Staffing labels

If a company is a subsidiary or establishment and its name contains the parent company’s name, Lightcast typically rolls it up into the parent.

*Example*: Walmart Canada -> Walmart

### Brand and Product Exceptions

Some organizations advertise job postings under product or brand names rather than the legal parent company. These are handled as exceptions:

Example: A posting listed as TikTok appears under ByteDance, Ltd, the parent employer.

Hospitals with distinct public identities may also appear under their parent organization in the taxonomy when appropriate.

## Industry Classification Methodology

### Granularity of Classification

Lightcast assigns each company to the most granular industry level possible

* NAICS 6-digit level, when determinable
* Fallback to NAICS 2-digit, when a detailed assignment cannot be reliably inferred

Although companies may operate across multiple industries, Lightcast currently assigns one primary industry code per company.

### Assignment Process

Industry codes are assigned through a detailed review of the company’s main website, using key informational sections to determine the most accurate industry.

*Example*: Amazon is assigned NAICS 459999 All Other Miscellaneous Retailers, the industry most representative of its core activity, even though individual establishments may operate in different industries.

### Keyword-Based Classification

Programmatic classification can also be applied using company-name keywords.

*Example*: Companies with **hospital** in their name may be assigned NAICS 622110 General Medical and Surgical Hospitals.

### Geographic Variations

Lightcast uses U.S. NAICS codes for both U.S. and Canadian companies. (Canada’s NAICS variant is not yet applied.) For the UK, Australia, New Zealand, and Singapore, Lightcast uses each region’s country specific SIC coding.

## Staffing Company Methodology

After normalization, companies are evaluated to determine whether they should be flagged as staffing organizations. This assessment is performed through qualitative research. A company is labeled as staffing if it is

* A true staffing or recruitment company, or A job board or brand operated by a staffing company

This designation allows users to filter job posting results based on whether they want to include or exclude staffing entities.
