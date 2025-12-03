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

**90-Government**

* Federal Government (901)
  * 9011-Federal Government, Civilian
  * 90114 / 901149-U.S. Postal Service
  * 90119 / 901199-Federal Government, Civilian (excluding postal service)
  * 9012 / 90120 / 901200-Federal Government, Military
* State Government (902)
  * 9026-Education and Hospitals (State Government)
  * 90261-Education (Sate Government)
    * 902611-Elementary and Secondary Schools
    * 902612-Colleges, Universities, and Professional Schools
    * 902619-Other Schools and Educational Support Services
  * 90262 / 902622-Hospitals (State Government)
  * 9029 / 90299 / 902999-State Government (excluding Education and Hospitals)
* Local Government (903)
  * 9036-Education and Hospitals (Local Government)
  * 90361-Education (Local Government)
    * 903611-Elementary and Secondary Schools
    * 903612-Colleges, Universities, and Professional Schools
    * 903619-Other Schools and Educational Support Services
  * 90362 / 903622-Hospitals (Local Government)
  * 9039 / 90399 / 903999-Local Government (excluding Education and Hospitals)

***Classification Examples***

Under the Lightcast hierarchy

* A state-run sewage treatment plant appears under 902999 (**State Government**, excluding **Education** and **Hospitals**).
* A federal court establishment, classified as 922110 in standard NAICS, appears under 901199 (**Federal Government**, **Civilian**).
* A local community college, normally under 611210, is reclassified as 903612.

## Implications

Because Lightcast reclassifies all public-sector establishments under NAICS 90

* The primary NAICS hierarchy (all sectors except 90) contains private-sector establishments only, including
  * 611 Educational Services
  * 62 Health Care and Social Assistance
* All establishments listed under standard NAICS 92 (Public Administration) are reassigned within Lightcast's Government NAICS hierarchy.

Lightcast follows this approach to maintain consistency with datasets such as CES, OES, and BEA, which apply the same classification convention.
