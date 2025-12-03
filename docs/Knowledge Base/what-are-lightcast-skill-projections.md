---
title: What Are Lightcast Skill Projections?
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Organizations and educators often face critical questions such as

* What skills will be in demand in the next two years?
* What knowledge should current first-year students acquire before they graduate?
* How can we stay informed about cutting-edge skill trends?

Customers who rely on Lightcast for labor-market insights frequently ask what is coming next. Current demand offers valuable context, but it does not fully capture what actions are needed to prepare for the future. As the labor market evolves rapidly, stakeholders need visibility into what will matter when today’s students graduate, when employers complete relocations and begin hiring, or when new corporate initiatives ramp up.

Understanding the future requires more than today’s job postings. It requires forward-looking intelligence. Skill Projections provide that visibility.

## What Are Skill Projections?

Skill Projections deliver national estimates of skill demand two years into the future. Updated quarterly, they help customers track emerging trends and understand how the market is shifting.

Lightcast generates these projections by combining multiple data sources job posting patterns, employment trends, taxonomy research, and historical growth behaviors. A machine learning model forecasts future demand by analyzing both long-term posting histories and broader market dynamics. Because online job postings can fluctuate, the model includes cleaning and normalization processes to ensure forecasts reflect real market signals rather than noise.

## Assumptions and Caveats

Predicting future demand comes with inherent constraints. Several considerations should guide interpretation:

**Expanding Labor Market**

The model forecasts future demand within a labor market that historically grows at approximately 6% per year (see employment projections). As a result, skill projections generally lean toward positive growth. Customers should consider how individual skills compare with the market as a whole, not just their absolute projected change.

**The multi-year model emphasizes long term trends**

The model relies on several years of data and prioritizes sustained patterns over short-term hype. It requires multiple months of consistent growth before adjusting forecasts. This means some heavily publicized skills may have lower projections than expected if they lack a sufficiently long track record. 

*Example*: **Prompt Engineering** appeared in fewer than 10 job postings before 2023. The model therefore does not project extreme growth based on a single year’s rapid increase. If the skill continues to expand beyond the ***hype cycle***, the forecasts will adjust accordingly. ----- cross link TBD

**Projections apply only to defined skills**

Forecasts are generated for skills already present in the labor market and represented in Lightcast taxonomies. The taxonomy team continuously researches new trends and incorporates new skills, but Skill Projections themselves are not designed to identify emerging skills.

## Additional Detail

The Skill Projection model is an ensemble of multiple machine learning algorithms, each contributing to the most accurate forecast for a given skill. Using historical job postings and established occupational attributes, the model estimates future demand based on five years of trend data.

To account for uncertainty, the model produces a range of potential outcomes. This range enables it to reflect long-term trends while still responding to sudden shifts such as the rapid rise of generative AI in 2023 or unexpected market declines.

## Skill Value & Market Comparison

To help customers interpret projection results, Lightcast provides both the forecasted percentage change in demand and a comparison to overall market growth.

Because the broader labor market is expanding, market relative context is essential. Each skill is assigned one of four categories:

* **Rapidly Growing**: Increasing much faster than the overall market
* **Growing**: Increasing faster than the market
* **Stable**: Growing at about the same pace as the market
* **Lagging**: Growing more slowly than the market or declining

<Image border={false} />

All percentage values for Projected Skill Growth and Growth Relative to the Market are rounded to the nearest tenth (for example, 24.5%).

<br />
