---
title: Lightcast NAICS
deprecated: false
hidden: false
metadata:
  robots: index
---
<br />

This article explains how Lightcast NAICS codes differ from the standard NAICS classification and the reasons behind those differences.

## Vintage

Lightcast transitioned to the 2022 NAICS classification with the 2023.3 datarun in July 2023. All dataruns from 2017.4 through 2023.2 use the 2017 NAICS classification.

## Lightcast NAICS Particularities

No public dataset uses NAICS in its fully standard form, and Lightcast is no exception. Lightcast modifies specific NAICS codes to ensure accuracy and usability based on data availability and reporting practices. Key differences include

**Agricultural Industries**

Lightcast consolidates all industry data under

* 111 (Crop Production) -> 111000
* 112 (Animal Production) -> 112000

This consolidation addresses significant data suppression in QCEW, where approximately 75% of agricultural data points for sub-national regions are unavailable. Users seeking more granularity should consult local QCEW data where available.

**Rail Transportation**

Lightcast uses a single aggregate code 482110 (Rail Transportation), combining NAICS 482111 and 482112. The BLS does not report data for 482111 and 482112, therefore, Lightcast adopts the classification used by the Railroad Retirement Board, which reports under 482110.

**Postal Service**

In Lightcast data 491110 (Postal Service) represents private-sector USPS contractors only. Actual USPS establishments appear under Lightcast code 901149.

**Notaries**

Lightcast does not include data for 541120 (Offices of Notaries) because the BLS does not publish any data for this category.

**Public-Sector Hierarchy**

Lightcast creates a separate hierarchy for all government-run establishments under NAICS 90 (Government).
Details are provided in the next section.

## Government NAICS

QCEW provides an ownership flag identifying establishments as private, federal, state, or local government. In standard NAICS, government-run establishments appear throughout the hierarchy.

To align with conventions used in CES, OES, and BEA datasets, Lightcast reclassifies all public-sector establishments into a dedicated Government NAICS hierarchy.

<br />
