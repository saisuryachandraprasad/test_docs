---
title: Job Postings Analytics (JPA) Methodology
deprecated: false
hidden: false
metadata:
  robots: index
---
In this this article you'll get to know how Lightcast collects, processes, and enriches job postings to create reliable, high-quality labor market insights.

Job postings should not be viewed as a direct count of job vacancies. While they are related, employer hiring practices such as reposting or advertising for brand visibility can affect the relationship. Job postings are best understood as a measure of employer recruiting activity.

## Aggregation

Lightcast collects job postings from more than 220,000 current and historical online sources around the world. These include job boards, company career pages, and other public employment sites.

After a site is identified as a valid source, a custom crawler (or spider) is built to visit the site regularly. The spider extracts job information and sends it to our database. Sites with frequent updates or many new jobs are visited more often.

To ensure complete coverage, we continue checking each site for up to 14 days after the initial crawl. Most postings appear in Lightcast data within 36 hours of being scraped and processed.

## Deduplication

Because job posts often appear on many websites, removing duplicates is critical. Lightcast uses a two-step deduplication process that removes up to 80% of duplicates

* **Source-level check**: Each crawler tracks which posts have already been collected from its site and ignores older copies.
* **Cross-site check**: Standardized fields-job title, employer, and location are compared across 60 days of data. Matching postings found on different sites are treated as duplicates.

<Accordion title="Example">
  If a company post a **Marketing Specialist** job on March 1, that is the original posting. Any matching versions found for the next 60 days count as duplicates. Even if that company reposts the job daily on multiple sites for a year, Lightcast would count it only about six times during that period.
</Accordion>

## Data Curation

Lightcast does not smooth posting trends. Instead, a consistent deduplication method keeps the dataset stable.

A small portion of postings (about 1% each month) is removed using a proprietary tool that detects misleading or low-quality posts.

**Examples include**

* Pay-to-work postings
* Pyramid scheme or MLM solicitations
* Sexually explicit or discriminatory postings
* Spam, including mass gig-economy or trucking postings

## Job Post Expiration

Lightcast determines when a job posting is no longer active using two methods:

* **Fetch-based expiration**: We revisit job post and look for messages such as **Page not found** or **This job is no longer active**.
* **Age-based expiration**: Any single advertisement expires after 60 days.

For postings built from multiple matching advertisements, we track all related postings and marks the posting expired once all associated ads have expired up to a maximum of 121 days.

<Accordion title="Example">
  Posting consists of two ads:

  * post 1: Posted Jan 1, expires Mar 2
  * Post 2: Posted Mar 2, expires May 1

  Therefore, job post is considered as **active** from **Jan 1** to **May 1**
</Accordion>

## Active & Newly Posted Metrics

* **Newly Posted**: The number of postings first published in a given month.
* **Active**: The number of postings that were live at any point during the month, even if they were originally posted earlier.

Newly Posted helps show change in employer activity. Active postings help show total demand.

## Enrichment

After aggregation and deduplication, each posting is enriched with dozens of data elements, including

* Standardized job titles and occupations
* Employer information
* Skills, certifications, and work activities
* Education requirements
* Experience levels
* Salary details (If provided)
* Number of openings and job type

This added detail helps users understand not just job counts, but the specific skills and qualifications employers want.

## Company Normalization

Lightcast cleans and standardizes raw employer names by removing terms like **LLC** or **Inc** and matching each company to the Lightcast Companies Taxonomy.

The taxonomy includes metadata such as

* Parent company
* Tradestyle
* NAICS codes
* Staffing labels

Subsidiaries are generally rolled up into the parent company unless they operate as their own brand (for example, Walmart Canada). Some brands such as **TikTok** are mapped to the parent company **ByteDance Ltd**. Hospitals may remain separate where appropriate.

> You can refer ***Industry Classification*** for detailed expiation ---- cross link TBD

## Education Level

Lightcast assigns education requirements using a machine-learning model. A posting may receive multiple education tags if several levels are mentioned. Possible values include

* High School/GED (General Educational Development)
* Associate’s Degree
* Bachelor’s Degree
* Master’s Degree
* PhD/Professional Degree
* Unspecified (if not stated)

> You will find detailed explanation ***here***     --------- Cross Link TBD

## Employment Type

Lightcast tags postings as

* Full-time (more than 32 hours)
* Part-time (32 hours or less)
* Flexible hours (mixed or variable schedules)
* Intern

If no type is listed, full-time is assumed.

## Experience

We capture required years of experience when provided. If a posting does not mention experience, it will not appear in filters that require minimum experience.

## Location

While scraping location details are collected as Country, state, and city. If multiple cities are listed, the first one is selected.

<Accordion title="Driver">
  Driver Wanted in London, OH, Logan, OH, Mount Gilead, OH.
  Locatio will be considered as London, OH
</Accordion>

Lightcast then maps city-state pairs to counties and MSAs (Metropolitan Statistical Area) using Google geocoding and internal mapping tools.

## Skills

We extract skills using the Lightcast Skills Taxonomy. On average, **13 skills** are identified per posting.

The model recognizes aliases, abbreviations, and historic names and uses context to ensure accuracy. For example, “AWS” could refer to “Amazon Web Services” or the “American Welding Society,” depending on surrounding text.

Each skill receives a confidence score, and only skills meeting quality thresholds are included.

> Check out Lightcast Skills Taxonomy ***here***   -------- Cross link TBD

## Advertised Salary

If salary information is present, Lightcast extracts and cleans it. It does not estimate salaries when none are provided.

Salaries are converted between hourly and annual formats using **standard work hours** for each country (for example, 2,340 hours per year in Turkey).

## Remote or Hybrid

Lightcast analyzes posting text to determine whether a job is Remote, Hybrid, or Non-Remote. Common signals include **work from home**, **telecommute**, or **can be located anywhere**.

Jobs that require living in a specific region but not attending an office are considered Remote. If the posting does not clearly state location details, the classification is Unknown.

## Titles

Titles are cleaned and mapped to the Lightcast Titles Taxonomy. Complex or brand-specific titles are simplified.

**Example**: Data Science Manager, Messenger, in Facebook job post would be normalized as **Data Science Manager**.

> Check out Lightcast Title Taxonomy ***here*** ----- cross link TBD

## Occupations

Occupations are assigned using a combination of curated rules and machine-learning models.

* Rules are applied first for consistent and known patterns.
* Machine learning evaluates postings without rule matches.
* Additional rules map the result to broader occupation taxonomies.

Lightcast continuously improves these rules and models with series of quality checks and manual reviews to support accuracy.

## Contract Type

Lightcast supports the following contract types:

* Apprenticeship
* Internship
* Temporary
* Temporary/Permanent
* Permanent

Apprenticeships and internships use machine-learning classification.

All postings default to Permanent unless language indicates for example, **seasonal**, **summer opportunity**, or **temp-to-hire**.

## Unclassified Postings

Some postings may remain unclassified if information is missing or the system cannot confidently assign a value. Lightcast monitors these cases and reduces them through ongoing monthly improvements.

## Job Posting Classifier Updates

Every month, we reprocess all historical and current postings using the latest classifiers. This includes

* Reclassification
* Deduplication
* Updated skills and taxonomies

For example, when the skill **Generative AI Agents** was introduced in January 2025, Lightcast retroactively identified it in all historical postings.

This process is seamless for customers and involves no downtime.

> You can explore our _**taxonomies**_ and _**postings changelogs**_ for details.      --------- Cross Link TBD

<br />
