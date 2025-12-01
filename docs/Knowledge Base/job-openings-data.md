---
title: Job Openings Data
deprecated: false
hidden: false
metadata:
  robots: index
---
Job Openings represent the total number of positions employers are expected to fill during a selected time period.
Openings are calculated as

`Growth + Replacements = Openings`

* Growth measures the net increase in employment for an occupation.
* Replacements measure the number of workers permanently leaving an occupation and needing to be replaced.

The sections below explain how both components are calculated.

## Replacement Jobs

Replacement demand comes from Lightcast job counts, and National occupation specific separation rates from the ***BLS Employment Projections program***. ---- Cross link TBD

**What Separations Include**

The BLS separations methodology counts workers who permanently leave an occupation, such as

* Retiring
* Switching to a different occupation

It does not count

* Workers moving to a new region but staying in the same occupation
* Workers changing employers but staying in the same role

**Why BLS Updated Its Methodology**

Before our 2017.3 datarun, the older BLS **Replacements** approach assumed workers stayed in the same occupation for an entire career. This led to

* Undercounting young workers leaving occupations
* Undercounting older workers entering new occupations
* Overall replacement needs being significantly underestimated

The updated Separations methodology corrects these issues and produces replacement figures that better reflect real labor market behavior.

> For more details about old & new methodology, you can check here ----- cross link TBD (one extra link for blog)

**How Replacements Are Calculated**

Replacements are calculated year by year, then summed across the selected timeframe.

Example: `2016 Replacements = 2016 Jobs × BLS Replacement Rate`

If a user selects 2013-2020, replacements for each year are added to produce the total.

## Growth

Growth is based on Lightcast occupational job counts. It's treated as a net term

* Positive employment change = growth
* Negative employment change = zero growth (no negative growth)

**Why Aggregation Matters**

Growth should be calculated before aggregating across

* Geographies (county -> state -> nation)
* Occupation levels
* Classes of worker
* Years

This prevents job losses in one area from canceling out job gains in another.

**Example**

At the state level, growth appears to be 300. But when calculated separately for each county

* County 1 shows significant job gains
* County 2 shows job losses

If only state level net growth is used, County 1’s opportunities are hidden behind County 2’s losses.

The correct method is to

1. Compute net new growth at the lowest level (e.g, county)
2. Sum the positive values across areas

Using this approach, the total becomes 1,000 rather than 300 accurately showing the opportunity available across counties.

**Key Takeaways**

For any aggregated region or range of years

* Total growth will always be equal to or greater than net job change.
* This ensures job openings reflect genuine labor demand rather than masking local opportunities.
