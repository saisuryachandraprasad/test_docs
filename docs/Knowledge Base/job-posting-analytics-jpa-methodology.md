---
title: How to Use Keyword Search
deprecated: false
hidden: false
metadata:
  robots: index
---
When the predefined categories aren’t flexible or specific enough, you can use keywords to filter job postings, profiles, and in some cases, compensation. Keywords are matched against the original text of job postings and profiles, and are also used by Lightcast's compensation model to find wage observations for specific skillsets. It is important to note the following with keyword searches:

* Whatever text is typed in the keyword box will be broken up into words using spaces and punctuation as boundaries.
* Letter capitalization is ignored.
* Very common words such as a, an, the, in, on, for, etc. --- known as “stopwords” --- will be ignored.
* Keyword searches work together with your other filters (such as region, ONET/SOC code, and skills).

Keyword search can be extremely powerful, allowing you to filter based on intricate combinations of words and phrases if you take some time to understand the queries.

1. **Default:**
   The basic use case is to search for a series of keywords (i.e. `history economics politics`); in this case the filter will require **all** of the keywords you entered (excluding stopwords). Alternate word tenses and plurality will match as well, so searching for `politics` will match “politics”, “politic”, “political”, etc.
2. **Special characters:**
   The following characters and words have a special meaning, and may cause your search to return unexpected results or an error if not used correctly: `+-"~() AND OR NOT`. In addition, the following characters are ignored in search text: `[]{}/\:<>^`
3. **Boolean expressions:**
   Use `AND`, `OR`, `NOT` (they must be capitalized) and parentheses to specify combinations of keywords. `AND` will be evaluated before `OR` if no parentheses are given. Two keywords separated by only a space will be assumed to have an `AND` between them.
   1. Example 1: `(drone OR UAV) AND agriculture` matches text that contains “agriculture” and either “drone” or “UAV” (unmanned aerial vehicle).
   2. Example 2: `(drone OR UAV) AND NOT surveillance` matches text that contains either “drone” or “UAV” and that does not contain the word “surveillance”.
4. **Quotes**** _:_**
   Double-quotes mark out phrases, allowing you to incorporate phrases into larger expressions.
   1. Example: `("degree in history" OR "degree in economics") AND "public policy"`.
5. **Stopwords:**
   All stopwords will be ignored from explicit matches. Instead, they will allow for **any** word to take their place in order to facilitate a match. For instance, searching for `"Degree in history"` will match “Degree in history”, “Degrees on history”, “Degrees about history”, etc. Searching for only stop words will not produce any matches. It's important to note that queries are case insensitive, so searches such as `"Portland, OR"` and `"System Administrator" AND IT` may not return exactly what you would expect, since “OR” and “IT” are both stop words.
6. **Simple inclusion and exclusion:**
   Place a plus sign “+” in front of any words that must be present and a minus sign “-” in front of any words that must not be present.
   1. Example: `+drones +agriculture -surveillance`
7. **Misspellings:**
   You can search for variant spellings by using the character “~” followed by a number, which we’ll call **N** , immediately after a word. This will search for the given word or any word that can be made with **N** changes to the original, where one change is (a) removing a character, (b) adding a character, (c) substituting a character, or (d) transposing two adjacent letters.
   1. Example: `theater~1` will match _theater_ , _theatre_ , and _thaeter_ ; but also _cheater_ , _heater_ , and _treater_.Example: `psychology~1` will match _sychology_ , _psycology_ , _psycholgy_ , _psycholigy_ , and _pyschology_ ; but not _sycology_.
8. **Phrase Proximity:**
   You can also search for phrase variants by using a phrase in double quotation marks followed immediately by a “~” and a number we can call **N**. This will search for the phrase with up to **N** changes to it, where a change is (a) adding a word between the original words, (b) removing a word, (c) substituting one word for another, or (d) swapping the order of two adjacent words. So the search `"history degree"~2` would match “history degree” (no changes), “degree in history” (two changes: swap word order and add a word between), “history or sociology degree” (two changes: add two words between), and so on.
   However, because phrase searches can cross sentence boundaries, it could also match unexpected text like “This is your chance to make history! Bachelor’s degree in computer science required…”, since the section “history! Bachelor’s degree” will be reduced behind the scenes to “history bachelors degree”, which is within 1 word change of the search phrase “history".
