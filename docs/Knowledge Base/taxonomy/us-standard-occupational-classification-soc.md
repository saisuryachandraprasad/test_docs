---
title: US Standard Occupational Classification (SOC)
excerpt: National Occupation Taxonomy of the United States
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

The Standard Occupational Classification (SOC) system is the framework used by U.S. federal statistical agencies to classify workers into occupational categories for data collection, analysis, and reporting. Every worker is assigned to one of 840 detailed occupations based on the official occupational definition.

To support consistent classification

* Detailed occupations are grouped into 461 broad occupations
* Broad occupations are grouped into 97 minor groups
* Minor groups roll up into 23 major groups

Occupations within the SOC are organized by similarities in job duties and, in some cases, required skills, education, or training. The SOC uses hyphenated codes to distinguish its four hierarchical levels: major groups, minor groups, broad occupations, and detailed occupations.

Example of SOC Structure

* 29-0000-Healthcare Practitioners and Technical Occupations (major group)
  * 29-1000-Health Diagnosing and Treating Practitioners (minor group)
    * 29-1020-Dentists (broad occupation)
      * 29-1021-Dentists, General (detailed occupation)
      * 29-1022-Oral and Maxillofacial Surgeons (detailed occupation)
      * 29-1023-Orthodontists (detailed occupation)
      * 29-1024-Prosthodontists (detailed occupation)
      * 29-1029-Dentists, All Other Specialists (detailed occupation)

**Differences Between Lightcast SOC Codes and Standard SOC**

While Lightcast aligns closely with the SOC system, several modifications are made where data limitations or modeling needs require it.

**Military Occupations**

Due to limited data availability, Lightcast does not assign individual SOC codes for military roles. All 20 military occupations are grouped under 55-9999.

**Postsecondary Teachers**

Lightcast uses a single aggregate code 25-1099 instead of the 38 detailed SOC codes for postsecondary instructors. This approach reflects data constraints and maintains alignment with the BLS National Industry Occupation Employment Matrix (NIOEM).

**Unclassified Occupations**

Lightcast adds 99-9999 Unclassified Occupation to represent Extended Proprietors in industries where occupational estimates cannot be reliably produced.

**Substitute Teachers**

Following OES methodology, Lightcast includes 25-3098 Substitute Teachers.

## Versions of SOC

The SOC system has evolved through several revisions. Lightcast products and federal datasets may reference different versions depending on the data year.

* **SOC 2018**-Used in Lightcast products beginning with the 2022.4 data run.
* SOC 2017-Adopted by OES starting with 2017 data; used by Lightcast beginning 2018.3.
* SOC 2010-Used by BLS for 2012 forward; Lightcast used this version from 2013.3 to 2018.2.
* SOC 2010 Transitional – Used for OES 2010 and 2011 data.
* SOC 2000 – Used in most BLS datasets from 2001 to 2009.
