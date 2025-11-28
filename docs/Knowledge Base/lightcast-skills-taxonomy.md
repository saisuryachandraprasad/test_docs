---
title: Lightcast Skills Taxonomy
deprecated: false
hidden: false
metadata:
  robots: index
---
Lightcast defines a skill as any competency or attribute an employer uses to differentiate roles or that a candidate uses to stand out in their career profile. The Lightcast Skills Taxonomy includes 33,000+ skills sourced from hundreds of millions of job postings and profiles. Skills are organized into a three-tier hierarchy

1. **Category**: broad groupings aligned roughly to ABC Career Areas.
2. **Subcategory**:  clusters of skills used for specific tasks or job functions.
3. **Skill**:  the individual competency.

**The taxonomy contains**

* Common Skills (e.g., communication, problem-solving)
* Specialized Skills (e.g., Java, financial analysis)
* Certifications and Licenses (e.g., CompTIA Security+, Certified Radiological Nurse)
* Languages and Software Skills

Most skills include a definition sourced from reputable references such as Wikipedia or Wiktionary. Lightcast taxonomists update the skill list continuously tracking new skills, aging skills, and user requests.

## Monthly Skill Refresh

Lightcast updates the Skills Taxonomy each month. During each refresh

* New skills may be added
* Outdated skills may be removed
* Terminology and coding may be revised

This ensures the library reflects current labor market language and emerging trends.

## Skills Coding Process

Each skill has one official display name. To improve detection accuracy in postings and profiles, the model also recognizes

* Aliases
* Abbreviations
* Acronyms
* Legacy or historic names

The extraction process includes 

1. Segmenting and tokenizing text to remove punctuation and formatting
2. Scanning for word sequences that match known skills
3. Using context to disambiguate similar terms
   1. Example: “AWS” may refer to Amazon Web Services or the American Welding Society
4. Assigning a confidence score
5. Displaying only skills that meet quality thresholds

> Customer support ----------- one line desc and cross link TBD
