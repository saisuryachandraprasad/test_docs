---
title: What are different types of Educational Attainment?
excerpt: >-
  This guide explains how educational attainment appears across Lightcast data
  sources, including U.S. public data, demographic data, and job postings.
deprecated: false
hidden: false
metadata:
  robots: index
---
## Education in U.S. Public Data

### Educational Attainment by SOC Code

**Geography**: National
**Definition**: Shows the education levels attained by workers employed in a specific occupation.
**Source**: Bureau of Labor Statistics (BLS), ***Education and Training Measurements for Workers 15 Years and Older by Detailed Occupation***. ----- cross link TBD
*Example*: Nearly 50% of Registered Nurses in the U.S. have a bachelor’s degree, while about 9% hold a master’s degree.

### Typical Entry-Level Education

**Geography**: National
**Definition**: Indicates the education level most people have when entering an occupation.
**Source**: BLS, ***Education and Training Measurements for Workers 15 Years and Older by Detailed Occupation***. -- cross link TBD
*Example*: Journalists typically enter the field with a bachelor’s degree, while environmental engineers may require a master’s or doctoral degree.

### Educational Attainment by Demographic

**Geography**: Regional (down to the county level)
**Definition**: Shows education levels by gender and race/ethnicity for the U.S. population ages 25 and older.
**Source**: Two years of microdata from the Census Bureau’s ***American Community Survey (ACS)***. -- cross link TBD
*Example*: In 2018, 28% of the U.S. population held a high school diploma: 52.5 million males and 55.2 million females.

### Educational Attainment by O*NET Code

**Geography**: National
**Definition**: Shows the education levels generally required for employment in an occupation. These requirements may differ from the actual education levels attained by workers (as reflected in BLS SOC-level data).
**Source**: ***O\*NET Database***. ---- cross link TBD
*Example*: Nationally, 23% of registered nurses might have a bachelor’s degree, while 66% hold an associate degree.

## Education in Job Postings

### Job Posting Analytics (JPA)–Education Level

**Geography**: Regional
**Definition**: Captures any education level mentioned in a posting. Requirements may be preferred, required, or negotiable, and postings may include multiple education levels.
**Source**: Education fields extracted from job postings collected by Lightcast.
*Example*: “A.A. or B.A. or equivalent experience preferred” is counted under both associate degree and bachelor’s degree.

### JPA–Minimum Education Required

**Geography**: Regional
**Definition**: Reflects the minimum education level explicitly required in a job posting. Postings with no stated education requirement are classified as Unspecified.
**Source**: Minimum education information extracted from job postings collected by Lightcast.
*Example*: “Bachelor’s minimum, postgraduate preferred” is counted as requiring a bachelor’s degree.
