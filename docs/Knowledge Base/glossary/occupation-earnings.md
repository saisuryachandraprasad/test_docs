---
title: Occupation Earnings
deprecated: false
hidden: false
metadata:
  robots: index
---
## Overview

Occupation earnings are sourced from the U.S. Bureau of Labor Statistics (BLS) Occupational Employment and Wage Statistics (OES) dataset. Because OES data is collected from the employer’s perspective, earnings are reported pre-tax and are attributed to the location of the job, not the employee’s residence.

The dataset provides average hourly earnings and percentile earnings for the 10th, 25th, 50th (median), 75th, and 90th percentiles.

## Understanding Earnings Measures

**Average Earnings**

Average earnings represent total earnings for all workers in an occupation divided by the total number of jobs. `total earnings of all workers /total number of jobs`

**Percentile Earnings**

Percentile earnings indicate the portion of workers earning a specific amount or less. For example,

* 10th percentile earnings of $12/hr indicate that 10% of workers earn $12 per hour or less.
* Median earnings of $15/hr mean that half of workers earn more and half earn less.

The 10th percentile is frequently used as a proxy for entry-level wages because it reflects earnings at the lower end of the distribution.

**Hourly** vs. **Annual Earnings**

Most occupations report earnings in hourly terms. For roles with annual reported earnings, Lightcast converts annual wages to hourly wages using a standard divisor of 2,080 hours (the estimated number of work hours in a full year).

### What's Included

Occupation earnings encompass a variety of income components the employer reports

* Base rate
* Commissions
* Cost-of-living allowances
* Deadheading pay
* Guaranteed pay
* Hazard pay
* Incentive pay
* Longevity pay
* Over-the-road pay
* Piece rates
* Portal-to-portal rates
* Production bonuses
* Tips

### What's Excluded

Certain payments and benefits are not included in occupation earnings, such as

* Attendance bonuses
* Back pay
* Clothing allowances
* Discounts and merchandise discounts
* Draw
* Holiday bonuses and holiday premium pay
* Jury duty pay
* Meal or lodging payments
* Non-production bonuses
* On-call pay
* Overtime pay
* Perquisites
* Profit sharing
* Relocation allowances
* Severance pay
* Shift differentials
* Stock bonuses
* Tool or equipment allowances
* Tuition reimbursement
* Uniform allowance
* Weekend premium pay
* Year-end bonuses

Definitions for all categories are provided in the _**OES documentation**_. ----cross link TBD

<Callout icon="💡" theme="default">
  **Canada Data Sources**

  For Canada, occupation earnings are derived from

  * Lightcast’s industry dataset
  * Regional occupation data from the Labour Force Survey (LFS)
  * Regional staffing patterns from the Census
</Callout>

## Percentile Earnings in Lightcast Tools

Lightcast's Analyst and Developer tools allow users to combine percentile earnings across occupations or regions. These combinations are generated using a proprietary occupation aggregation methodology designed to model combined wage curves more accurately than a simple weighted average.

Because of this approach, manually combining percentile earnings will not match the combined figures displayed in Analyst. More details on Lightcast's percentile earnings methodology are available _**here**_. ------cross link TBD

> Lightcast's proprietary employment data, based primarily on occupational earnings reported in the OES dataset.

<br />
