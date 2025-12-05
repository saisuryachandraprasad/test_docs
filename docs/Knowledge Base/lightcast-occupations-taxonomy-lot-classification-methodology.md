---
title: Lightcast Occupations Taxonomy (LOT) Classification Methodology
deprecated: false
hidden: false
metadata:
  robots: index
---
The Lightcast Occupations Taxonomy (LOT) Classifier identifies LOT Specialized Occupations using a curated machine learning approach.

The model analyzes a job posting’s title, description, and regional context (such as country of origin and language) to classify the posting into one of Lightcast's Specialized Occupations. Portions of the model are curated by taxonomists to ensure accurate recognition of occupation-specific keywords, skills, and terminology. The remainder of the model is trained on a large corpus of raw job postings to capture

* Relevant skills
* Industry certifications
* Representative duties and responsibilities
* Terminology unique to specific roles or sectors

Before classification, the model removes common words, company boilerplate language, and benefit descriptions to prevent noise in the prediction process.

Once the posting is assigned to a Specialized Occupation within the Taxonomy, it can be mapped to a national occupation taxonomy such as O*NET, UKSOC, or NOC. The LOT classifier generates both occupation names and codes using Lightcast's hierarchical structure

* Career Area
* Occupation Group
* Occupation
* Specialized Occupation

From these structured outputs, corresponding national taxonomy codes can be derived.
