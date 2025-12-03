---
title: 'Global Postings Data '
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Lightcast Global’s job postings data is sourced from a wide range of regions and platforms. While country availability varies by product, ABC maintains profile data for more than 150 countries.

<Callout icon="⚙️">
  Real time labor market insights covering more than one-third of the global workforce.
</Callout>

## Data Collection

Lightcast collects demand data daily from global sources. Whenever possible, we prioritize primary sources, including

* Applicant tracking systems (ATS)
* Direct employer postings on job boards

These are supplemented with high quality secondary sources to strengthen coverage.

Because employers use diverse languages, conventions, and terminology, our global and linguistics teams clean, enrich, and classify postings using Lightcast taxonomies. We also deduplicate postings each day and incrementally update the dataset. All demand data is refreshed bi-weekly with the latest enrichments.

This end-to-end process standardizes postings across countries and markets, enabling consistent global analysis.

Lightcast demand data is available through

* Global Talent Analyst --- cross link TBD
* Spotlight --- cross link TBD
* Lightcast APIs --- cross link TBD
* Snowflake --- cross link TBD

## Skills --- cross link TBD

Skills serve as a universal translation layer that enables consistent interpretation of job requirements across languages and cultures. To support accurate analysis

* Lightcast does not translate non-English postings.
* Skills are extracted in the posting’s native language, ensuring contextual relevance.

Skills help analysts understand global labor markets through

* **Granularity**: Skills provide detailed insights beyond job titles.
* **Comparability**: Skills function as a universal framework across countries.
* **Future-orientation**: Skills reveal emerging capabilities and labor trends.

Incorporating skills into demand analysis enables more precise, context-aware decisions.

## Companies --- cross link TBD

Lightcast normalizes company names across postings to enable accurate identification of employers hiring in specific markets. After cleaning and tagging, company information can be used to

* Analyze competitor hiring strategies
* Track posting intensity by employer or region
* Improve classification accuracy for international datasets

Normalized company data ensures consistent interpretation across geographies.

## Occupations --- cross link TBD

Global demand data is currently tagged using the ***Lightcast Occupation Taxonomy (LOT)***, Lightcast's proprietary, multi-level occupational framework. LOT identifies equivalent roles across employers and regions, even when job titles vary particularly important in emerging fields. --- cross link TBD

LOT includes four hierarchical levels

* Career Area
* Occupation Group
* Lightcast Occupation
* Specialized Occupation

<Callout icon="💡">
  The previous ***Global Occupations taxonomy*** is still present but will eventually be deprecated. Users are encouraged to migrate to LOT because it is ------ cross link TBD

  * More granular
  * More accurate
  * More reflective of current labor market dynamics
</Callout>

## Advertised Wage --------- cross link TBD

Wages listed in job postings can reveal compensation expectations for specific roles, regions, and skills. They can also indicate which occupations are viewed as especially valuable in a given market.

However, wage data should be interpreted with caution. Local norms, cultural expectations, and posting conventions can vary widely and are difficult to capture in a single number. For this reason, advertised wage analysis is most effective at a granular level.
