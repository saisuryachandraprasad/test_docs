---
title: How to Use Keyword Search
deprecated: false
hidden: false
metadata:
  robots: index
---
Keyword search allows you to filter job postings, worker profiles, and in some cases compensation results when predefined categories are not flexible or specific enough. Keywords are matched against the original text of postings and profiles, and they are also used by Lightcast's compensation model to identify wage observations associated with particular skill sets.

Before constructing queries, it is important to understand how keyword search interprets text.

**How Keyword Search Processes Text**

* Tokenization: All text you enter is split into individual words using spaces and punctuation.
* Case Insensitivity: Capitalization is ignored.
* Stopwords Removed: Extremely common words such as a, an, the, in, on, for, and others are ignored during matching.
* Works With Other Filters: Keyword search combines with your other filters, such as region, SOC/ONET code, and skills.

**Basic Keyword Search**

The default behavior is to find records containing all the keywords you enter (excluding stopwords).

*Example*: `history economics politics`
returns results containing all three terms. Variations in tense and plurality will also match, for example, politics will match political or politic.

**Special Characters**

The following characters have special meaning and may produce unexpected results if not used correctly

`+ - " ~ ( ) AND OR NOT`

The characters listed below are ignored entirely when included in search text:

`[ ] { } / \ : \< > ^`

**Boolean Expressions**

Use Boolean operators to create more precise queries

* AND: requires both terms
* OR: allows either term
* NOT: excludes terms

Operators must be capitalized. If no operator is written, a space between terms is treated as AND. Parentheses control grouping and evaluation order. When parentheses are not used, AND is evaluated before OR.

*Example 1*: `(drone OR UAV) AND agriculture`
Matches text containing agriculture and either drone or UAV.

*Example 2*: `(drone OR UAV) AND NOT surveillance`
Matches text that includes drone or UAV but excludes surveillance.

**Quoted Phrases**

Use double quotes to search for exact phrases.

*Example*: ("degree in history" OR "degree in economics") AND "public policy"

**Stopwords**

Stopwords are ignored in explicit matches. This means any word can replace a stopword position while still generating a match.

*Example*: Degree in history
matches “Degree in history,” “Degrees on history,” “Degrees about history,” and similar variations.

Searching only stopwords will return no matches. Because stopwords are case-insensitive, queries like "Portland, OR" or "System Administrator" AND IT may produce unexpected results, as “OR” and “IT” are stopwords.

**Simple Inclusion and Exclusion**

Use the plus sign (+) to require a term and the minus sign (–) to exclude a term.

*Example*: `+drones +agriculture -surveillance`

**Handling Misspellings (Fuzzy Search)**

Append ~N immediately after a word to allow up to N character changes (add, remove, substitute, or transpose).

*Example*: `theater~1` matches theater, theatre, thaeter, but also cheater, heater, treater.

*Example*: `1psychology~1` matches sychology, psycology, psycholgy, psycholigy, pyschology, but not sycology.

**Phrase Proximity (Fuzzy Phrase Matching)**

Place a phrase in quotes, followed by ~N, to allow up to N changes such as

* Adding a word
* Removing a word
* Replacing a word
* Reordering adjacent words

*Example*: "history degree"~2

matches

* “history degree”
* “degree in history”
* “history or sociology degree”
* and similar variants

Because phrase matching can cross sentence boundaries, it may also match unintended text. For example:

* “This is your chance to make history! Bachelor’s degree in computer science required…” is internally reduced to “history bachelors degree,” which is close enough to match "history degree"~2.
