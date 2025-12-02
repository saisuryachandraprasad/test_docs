---
title: Industry Projections Methodology
deprecated: false
hidden: false
metadata:
  robots: index
---
Lightcast's industry projections are developed using Lightcast final industry data. This data is primarily sourced from the U.S. Bureau of Labor Statistics (BLS) Quarterly Census of Employment and Wages (QCEW), supplemented with additional datasets that cover industries not represented in QCEW.

## Projection Framework

Industry projections are calculated for each 6-digit NAICS code and county combination. For every county industry pair, Lightcast generates three 10-year projections based on 5, 10, and 15 years of historical employment data.

**Step 1**: **Identify Historical Trends**

Three historical trend lines are created one each for the 5-year, 10-year, and 15-year employment histories.

<Image border={false} />

**Step 2**: **Extend Trend Lines**

Each trend line is then projected 10 years into the future. These projections are extrapolations of the historical patterns.

<Image border={false} />

**Step 3**: **Combine and Apply Dampening**

The three projections are combined into a single forecast. A dampening factor is applied to moderate extreme growth or decline, ensuring that projected changes become progressively less aggressive over time.

<Image border={false} />

## Adjustments Using External Data

After creating the preliminary projection using Lightcast data, additional adjustments are applied using authoritative external sources.

**National Industry-Occupation Employment Matrix (NIOEM)**

Lightcast aligns projections to BLS national level figures by applying the year-over-year percentage changes reflected in the NIOEM dataset.

> NIOEM includes ***National Level Employment Projection Data*** as well ------ cross link TBD

**State Published Long Term Industry Projections**

Most states release long-term industry outlooks approximately every two years. Lightcast incorporates these state-level totals into the projection model and assigns weights based on the recency of the state's data

* More recent projections receive higher weight.
* Older projections receive lower weight.

These adjustments ensure that county-level projections remain consistent with broader national and state trends.

## Final Output

After integrating Lightcast data with national and state projections, the result is a calibrated and balanced set of Lightcast industry projections.

<Image border={false} />

<Callout icon="⚙️" theme="default">
  **Sources**

  * BLS Quarterly Census of Employment and Wages (QCEW) --------- cross link TBD
  * National Industry–Occupation Employment Matrix (NIOEM) --------- cross link TBD
  * State industry projections (e.g., Illinois) --------- cross link TBD
</Callout>
