---
title: Understanding Shift Share
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Shift-share is an economic tool that helps identify which industries or occupations are competitive in a region. It compares actual local job growth to expected growth based on national trends. It appears in the Industry Table, Occupation Table, and Program Table in ***Analyst and Developer***. --- cross link TBD

If an industry grows faster locally than nationally, that growth may be driven by unique regional advantages.
If it grows slower, the region may be underperforming relative to national conditions.

## The Four Components of Shift-Share

Shift-share analysis includes four parts

1. Industrial Mix Effect
2. National Growth Effect
3. Expected Change
4. Competitive Effect

These components help separate national trends from local strengths or weaknesses.

> Examples below use industry data, but the approach also applies to occupations.

## Industrial Mix Effect

The industrial mix effect estimates how many jobs an industry should gain or lose in your region based on how that industry is performing nationally.

**How It’s Calculated**

1. Calculate the industry premium `Industry Growth Rate – National Economy Growth Rate = Industry Premium`
2. Apply that premium to the number of regional industry jobs `Industry Premium × Regional Jobs = Industrial Mix Effect`

If the industry is growing nationally, similar growth is expected locally. If declining nationally, local decline is also expected.

## National Growth Effect 

The national growth effect measures how many jobs an industry is expected to gain or lose because the national economy is expanding or contracting. This is the **rising tide lifts all boats** effect.

**Calculation**: `National Growth Rate × Regional Jobs = National Growth Effect`

This effect is driven purely by overall U.S. job growth, not industry specific factors.

## Expected Change

Expected change combines both national influences 

**Calculation**:`Industrial Mix Effect + National Growth Effect = Expected Change`

This represents the amount of growth (or decline) we would anticipate before considering regional uniqueness. Any job change beyond this number becomes the competitive effect.

## Competitive Effect

The competitive effect measures how much job change in a region is due to local strengths or weaknesses not national trends.

**Calculation**: `Actual Regional Job Change – Expected Change = Competitive Effect`

* **Positive competitive effect**: The region is outperforming national expectations.
* **Negative competitive effect**: The region is underperforming relative to the nation.

A region may show positive competitive effect even during job decline if local job losses are smaller than national job losses.

<Accordion title="Examples" icon="fa-info-circle">

**Chicago Metro Area**

A chart of four industries in Chicago shows:

<Image border={false} />

* Warehouse clubs and supercenters
  * Positive competitive effect -> outperforming national trends.
* Elementary and secondary schools
  * Negative competitive effect -> underperforming national trends.

**Boston R&D Industry**

The R&D industry is declining nationally. Based on this

<Image border={false} />

Expected national decline in Boston: –120 jobs

Expected national economic growth contribution: +394 jobs

Expected change: `–120 + 394 = +274 jobs`

Actual growth was +1,459 jobs.

So, the competitive effect is: `1,459 – 274 = +1,186 jobs`

This means most of the growth is driven by Boston’s unique regional advantages, not national factors.

</Accordion>

**Boston Hospitals**

National trends predicted ~1.6K new hospital jobs. Actual change was 507 jobs.

Competitive effect: `507 – 1,596 = –1,088 jobs`

The region is underperforming national expectations, indicating local challenges.

<Image border={false} />

## Using Shift Share Analysis

Shift share helps highlight why industries grow or shrink locally something raw job counts alone cannot explain. This supports better decision-making for

* Regional planners
* Talent strategy leaders
* Colleges and universities
* Workforce development teams

> Shift share is similar location quotient, ***check here*** for detailed explanation --- Cross link TBD

**How Shift Share Helps**

* A booming industry may not be competitive locally if it’s booming everywhere.
* A declining industry may still be competitive locally if it’s declining less than the nation.
* Unexpectedly strong or weak performance can point to regional advantages or challenges that require further investigation.

<Callout icon="⚙️">
  - Shift-share can be applied at the occupation level, since occupational trends often mirror the industries that employ them.
  - You can move between industry and occupation analysis using staffing patterns and inverse staffing patterns in Analyst.
</Callout>
