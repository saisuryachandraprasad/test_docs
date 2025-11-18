---
title: Free API Features
deprecated: false
hidden: false
metadata:
  robots: index
---
Our Open Skills program provides free access to Skills and Titles APIs. These APIs give you a standardized way to describe skills and job titles across your systems.

> You can learn more about the Skills API here

## Why Use a Standard Taxonomy?

A clear, market-aligned taxonomy is the fastest way to bring structure to inconsistent or ungoverned data. we maintain and update Skills and Titles list regularly, allowing your teams to use a living, authoritative reference library that:

| Highlights                          | Description                                                                                           |
| :---------------------------------- | :---------------------------------------------------------------------------------------------------- |
| **Reduces free-text issues**        | Users select from a single, verified list instead of entering their own variations.                   |
| **Strengthens data governance**     | Each term includes a machine-readable ID, enabling accurate filtering, sorting, and reporting.        |
| **Improves search and discovery**   | Autocomplete and type-ahead help users find the correct term without memorizing spellings.            |
| **Enables analytics and reporting** | Consistent IDs allow you to group and analyze skills or titles by category, region, or business unit. |

> A clean taxonomy is essential for any skills intelligence initiative. Without it, downstream insights and reporting cannot be trusted.

## Use Cases

<Accordion title="Skill Inventory" icon="fa-info-circle">
  **Challenge**

  A global defense contractor needed a unified view of employee capabilities. Skills were collected from resumes stored in different formats, described with inconsistent terminology, and incompatible across systems. Leadership could not answer fundamental questions such as

  * How many employees have aircraft mainframe expertise?
  * How many employees have expertise in propulsion system design?
  * Which roles require proficiency in flight control systems?

  The People Analytics team required a scalable way to build a consistent skills inventory.

  **Solution**

  **1. Taxonomy-Driven Tagging**

  The Lightcast skill hierarchy (Skill -> Skill Sub-Category -> Skill Category) provides clear structure.

  Example: Flight Safety -> Air Transportation -> Transportation, Supply Chain & Logistics.

  **2. Skills Inventory Dashboards**

  As each employee is mapped to a consistent Skill ID and hierarchy, analysts can view the workforce by:

  1. Individual skills (for example, Pitot Static)

  2. Sub-categories (Air Transportation)

  3. Broad categories (Transportation, Supply Chain & Logistics)

  **3. Resume Skill Extraction**

  New or existing resumes can be processed through the free Skills API. The API automatically assigns standardized Skill IDs, reducing manual tagging effort and improving accuracy.
</Accordion>

<Accordion title="Title Standardization" icon="fa-info-circle">
  **Challenge**

  A multinational engineering organization struggled with thousands of inconsistent job title variants, such as “Sr. HVAC Eng.” or “Hydraulics Guru.” These inconsistencies affected reporting accuracy, internal mobility, and cross-regional talent benchmarking.

  **Solutions**

  1.Type-Ahead Autocomplete\*\*

  The Lightcast library of 75,000 standardized titles is integrated directly into CRM and HRIS title fields. Users select a single authoritative title instead of entering free-text variations.

  **2. Historical Title Normalization**

  The team used up to 50 free title normalizations per month to clean historical data. The Titles API automatically mapped inconsistent or misspelled titles to the correct Lightcast Title IDs. This automated approach standardized years of records within days.

  3. Governance and Reporting Dashboards\*\*

  With each record linked to a unique Title ID, workforce teams can reliably roll up and compare data by discipline (for example, Civil Engineer vs. Electrical Engineer), region, or business unit.
</Accordion>

## Features & Limits

| Feature                       | Benefit                                                             | Limits                                         |
| :---------------------------- | :------------------------------------------------------------------ | :--------------------------------------------- |
| 75,000 Titles & 33,000 Skills | Eliminates free-text issues; records become query-ready             | No title–skill linkage included                |
| Skill hierarchy               | Clean roll-ups by Skill -> Sub-Category -> Category                 | Market context not included                    |
| Autocomplete / type-ahead     | Users find the right term quickly, keeps new data clean             | Requires development effort                    |
| 50 free API calls / month     | Run pilot projects, tag resumes, and clean legacy titles at no cost | Hard monthly cap, upgrade if required for more |

<br />

<br />
