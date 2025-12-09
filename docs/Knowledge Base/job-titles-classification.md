---
title: Job Titles Classification
excerpt: How Lightcast Job Titles Classification Works
deprecated: false
hidden: false
metadata:
  robots: index
---
The Titles Classifier processes raw job titles those taken directly from sources such as job postings or resumes and maps them to one of more than 70,000 standardized Lightcast Titles. A raw title is unprocessed text from an external source, while a Lightcast Title is a curated, standardized title created from analyzing many raw-title variations.

**How the Classification Process Works**

The Titles Classifier uses a vector-based machine learning model to match raw job titles to the most appropriate Lightcast Title. Before vectorization

* Raw titles are normalized to remove noise and irrelevant details.

The model is trained on

* A large set of raw job titles
* The complete Lightcast Titles taxonomy

This training enables the model to

* Recognize duplicated or equivalent titles
* Understand relationships between titles and their acronyms, abbreviations, and semantic variations

**Classification Output**

The classifier returns the top matching Lightcast Titles along with similarity scores, indicating how closely each standardized title aligns with the raw title being analyzed.
