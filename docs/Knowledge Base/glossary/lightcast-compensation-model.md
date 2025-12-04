---
title: Lightcast Compensation Model
deprecated: false
hidden: false
metadata:
  robots: index
---
The Lightcast compensation model provides occupational wage estimates enhanced with skill- and certification-based wage premiums. It combines percentile wage data from Lightcast’s LMI-derived government sources with wage observations extracted directly from job postings.

## Sources

The compensation model integrates wage information from two primary sources:

**Occupational Employment and Wage Statistics (OEWS)**

The core of Lightcast’s occupational wage data is the Bureau of Labor Statistics (BLS) Occupational Employment and Wage Statistics (OEWS) dataset. OEWS is updated annually and provides percentile wage estimates for occupations at the metropolitan level across the United States.

When OEWS suppresses certain percentile estimates for confidentiality reasons, Lightcast applies internal unsuppression methods to produce complete occupation-level wage distributions.

**Job Postings**

Job postings supplement OEWS data by providing wage observations tied to specific skills and certifications, which OEWS does not capture. These postings are collected from online sources and processed through Lightcast’s job-posting pipeline.

For additional details, see

* Job Postings methodology for information on how postings are collected and processed
* Compensation inclusions for details on what is included in wage calculations
