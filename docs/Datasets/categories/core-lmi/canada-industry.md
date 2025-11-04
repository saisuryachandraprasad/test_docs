---
title: Canada Industry
deprecated: false
hidden: false
metadata:
  robots: index
---
## Introduction

The Canada Industry dataset provides essential insights into **Canadian labor market**, offering both historical and projected data on industry employment and earnings. It enables users to analyze workforce trends, evaluate economic performance, and compare industries across regions and time period. It covers historical data since **2001** to **current industry year** and project data for current industry year.

> _Current Industry Year refers to most recent year with more than six months of data available from [SEPH](https://kb.lightcast.io/en/articles/7934179-survey-of-enrollment-payrolls-and-hours-seph). It may differ from calendar year_.

## Popular Use Cases

you can use this dataset to:

* Identify high growth industries across Canada
* compare earnings by region and industry
* Understand workforce composition and trends by industry

## Metrics

This dataset includes following core metrics:

* jobs: Total number of occupied positions.
* Earnings: Total earnings for the industry since 2001 to current year.
* EPW: Earnings per worker since 2001 to current year / Total number of occupied positions.

> _One worker might fill more than one position_.

## Filters

you can use following dimensions to filter dataset.

* Class of Worker
* Area (Hierarchy: Nation, Province, Census Division, and Census Sub-division)
* Industry (2 to 4 digits <Anchor label="NAICS" target="_blank" href="https://kb.lightcast.io/en/articles/7934064-north-american-industry-classification-system-naics">NAICS</Anchor>)
* Year

```json Dimensions
[
   {
      "name": "Area",
      "levelsStored": [
         "0",
         "1",
         "2",
         "3"
      ]
   },
   {
      "name": "ClassOfWorker",
      "levelsStored": [
         "1"
      ]
   },
   {
      "name": "Industry",
      "levelsStored": [
         "0",
         "1",
         "2",
         "3"
      ]
   }
]
```

## Metadata

|                       |                                                                                     |
| :-------------------- | :---------------------------------------------------------------------------------- |
| Access                | [Core LMI API](https://docs.lightcast.io/lightcast-api/reference/overview-core-lmi) |
| Dataset Id            | `EMSI.ca.Industry`                                                                  |
| Dataset URL           | `https://agnitio.emsicloud.com/meta/dataset/EMSI.ca.Industry/{version}`             |
| Geographical Coverage | Canada (Hierarchy: Nation, Province, Census Division, and Census Sub-division)      |
| Data Size             | 1 GB                                                                                |
| Format                | Json                                                                                |
| Update Frequency      | Quarterly                                                                           |

<br />

### Versions

```json 2025.3
[
   {
      "name": "Jobs.2001"
   },
   {
      "name": "Jobs.2002"
   },
   {
      "name": "Jobs.2003"
   },
   {
      "name": "Jobs.2004"
   },
   {
      "name": "Jobs.2005"
   },
   {
      "name": "Jobs.2006"
   },
   {
      "name": "Jobs.2007"
   },
   {
      "name": "Jobs.2008"
   },
   {
      "name": "Jobs.2009"
   },
   {
      "name": "Jobs.2010"
   },
   {
      "name": "Jobs.2011"
   },
   {
      "name": "Jobs.2012"
   },
   {
      "name": "Jobs.2013"
   },
   {
      "name": "Jobs.2014"
   },
   {
      "name": "Jobs.2015"
   },
   {
      "name": "Jobs.2016"
   },
   {
      "name": "Jobs.2017"
   },
   {
      "name": "Jobs.2018"
   },
   {
      "name": "Jobs.2019"
   },
   {
      "name": "Jobs.2020"
   },
   {
      "name": "Jobs.2021"
   },
   {
      "name": "Jobs.2022"
   },
   {
      "name": "Jobs.2023"
   },
   {
      "name": "Jobs.2024"
   },
   {
      "name": "Jobs.2025"
   },
   {
      "name": "Jobs.2026"
   },
   {
      "name": "Jobs.2027"
   },
   {
      "name": "Jobs.2028"
   },
   {
      "name": "Jobs.2029"
   },
   {
      "name": "Jobs.2030"
   },
   {
      "name": "Jobs.2031"
   },
   {
      "name": "Jobs.2032"
   },
   {
      "name": "Jobs.2033"
   },
   {
      "name": "Earnings.2001"
   },
   {
      "name": "Earnings.2002"
   },
   {
      "name": "Earnings.2003"
   },
   {
      "name": "Earnings.2004"
   },
   {
      "name": "Earnings.2005"
   },
   {
      "name": "Earnings.2006"
   },
   {
      "name": "Earnings.2007"
   },
   {
      "name": "Earnings.2008"
   },
   {
      "name": "Earnings.2009"
   },
   {
      "name": "Earnings.2010"
   },
   {
      "name": "Earnings.2011"
   },
   {
      "name": "Earnings.2012"
   },
   {
      "name": "Earnings.2013"
   },
   {
      "name": "Earnings.2014"
   },
   {
      "name": "Earnings.2015"
   },
   {
      "name": "Earnings.2016"
   },
   {
      "name": "Earnings.2017"
   },
   {
      "name": "Earnings.2018"
   },
   {
      "name": "Earnings.2019"
   },
   {
      "name": "Earnings.2020"
   },
   {
      "name": "Earnings.2021"
   },
   {
      "name": "Earnings.2022"
   },
   {
      "name": "Earnings.2023"
   },
   {
      "name": "Earnings.2024"
   },
   {
      "name": "EPW.2001"
   },
   {
      "name": "EPW.2002"
   },
   {
      "name": "EPW.2003"
   },
   {
      "name": "EPW.2004"
   },
   {
      "name": "EPW.2005"
   },
   {
      "name": "EPW.2006"
   },
   {
      "name": "EPW.2007"
   },
   {
      "name": "EPW.2008"
   },
   {
      "name": "EPW.2009"
   },
   {
      "name": "EPW.2010"
   },
   {
      "name": "EPW.2011"
   },
   {
      "name": "EPW.2012"
   },
   {
      "name": "EPW.2013"
   },
   {
      "name": "EPW.2014"
   },
   {
      "name": "EPW.2015"
   },
   {
      "name": "EPW.2016"
   },
   {
      "name": "EPW.2017"
   },
   {
      "name": "EPW.2018"
   },
   {
      "name": "EPW.2019"
   },
   {
      "name": "EPW.2020"
   },
   {
      "name": "EPW.2021"
   },
   {
      "name": "EPW.2022"
   },
   {
      "name": "EPW.2023"
   },
   {
      "name": "EPW.2024"
   }
]
```
```json 2025.1
[
   {
      "name": "Jobs.2001"
   },
   {
      "name": "Jobs.2002"
   },
   {
      "name": "Jobs.2003"
   },
   {
      "name": "Jobs.2004"
   },
   {
      "name": "Jobs.2005"
   },
   {
      "name": "Jobs.2006"
   },
   {
      "name": "Jobs.2007"
   },
   {
      "name": "Jobs.2008"
   },
   {
      "name": "Jobs.2009"
   },
   {
      "name": "Jobs.2010"
   },
   {
      "name": "Jobs.2011"
   },
   {
      "name": "Jobs.2012"
   },
   {
      "name": "Jobs.2013"
   },
   {
      "name": "Jobs.2014"
   },
   {
      "name": "Jobs.2015"
   },
   {
      "name": "Jobs.2016"
   },
   {
      "name": "Jobs.2017"
   },
   {
      "name": "Jobs.2018"
   },
   {
      "name": "Jobs.2019"
   },
   {
      "name": "Jobs.2020"
   },
   {
      "name": "Jobs.2021"
   },
   {
      "name": "Jobs.2022"
   },
   {
      "name": "Jobs.2023"
   },
   {
      "name": "Jobs.2024"
   },
   {
      "name": "Jobs.2025"
   },
   {
      "name": "Jobs.2026"
   },
   {
      "name": "Jobs.2027"
   },
   {
      "name": "Jobs.2028"
   },
   {
      "name": "Jobs.2029"
   },
   {
      "name": "Jobs.2030"
   },
   {
      "name": "Jobs.2031"
   },
   {
      "name": "Earnings.2001"
   },
   {
      "name": "Earnings.2002"
   },
   {
      "name": "Earnings.2003"
   },
   {
      "name": "Earnings.2004"
   },
   {
      "name": "Earnings.2005"
   },
   {
      "name": "Earnings.2006"
   },
   {
      "name": "Earnings.2007"
   },
   {
      "name": "Earnings.2008"
   },
   {
      "name": "Earnings.2009"
   },
   {
      "name": "Earnings.2010"
   },
   {
      "name": "Earnings.2011"
   },
   {
      "name": "Earnings.2012"
   },
   {
      "name": "Earnings.2013"
   },
   {
      "name": "Earnings.2014"
   },
   {
      "name": "Earnings.2015"
   },
   {
      "name": "Earnings.2016"
   },
   {
      "name": "Earnings.2017"
   },
   {
      "name": "Earnings.2018"
   },
   {
      "name": "Earnings.2019"
   },
   {
      "name": "Earnings.2020"
   },
   {
      "name": "Earnings.2021"
   },
   {
      "name": "Earnings.2022"
   },
   {
      "name": "Earnings.2023"
   },
   {
      "name": "Earnings.2024"
   },
   {
      "name": "EPW.2001"
   },
   {
      "name": "EPW.2002"
   },
   {
      "name": "EPW.2003"
   },
   {
      "name": "EPW.2004"
   },
   {
      "name": "EPW.2005"
   },
   {
      "name": "EPW.2006"
   },
   {
      "name": "EPW.2007"
   },
   {
      "name": "EPW.2008"
   },
   {
      "name": "EPW.2009"
   },
   {
      "name": "EPW.2010"
   },
   {
      "name": "EPW.2011"
   },
   {
      "name": "EPW.2012"
   },
   {
      "name": "EPW.2013"
   },
   {
      "name": "EPW.2014"
   },
   {
      "name": "EPW.2015"
   },
   {
      "name": "EPW.2016"
   },
   {
      "name": "EPW.2017"
   },
   {
      "name": "EPW.2018"
   },
   {
      "name": "EPW.2019"
   },
   {
      "name": "EPW.2020"
   },
   {
      "name": "EPW.2021"
   },
   {
      "name": "EPW.2022"
   },
   {
      "name": "EPW.2023"
   },
   {
      "name": "EPW.2024"
   }
]
```
```json 2024.3
[
   {
      "name": "Jobs.2001"
   },
   {
      "name": "Jobs.2002"
   },
   {
      "name": "Jobs.2003"
   },
   {
      "name": "Jobs.2004"
   },
   {
      "name": "Jobs.2005"
   },
   {
      "name": "Jobs.2006"
   },
   {
      "name": "Jobs.2007"
   },
   {
      "name": "Jobs.2008"
   },
   {
      "name": "Jobs.2009"
   },
   {
      "name": "Jobs.2010"
   },
   {
      "name": "Jobs.2011"
   },
   {
      "name": "Jobs.2012"
   },
   {
      "name": "Jobs.2013"
   },
   {
      "name": "Jobs.2014"
   },
   {
      "name": "Jobs.2015"
   },
   {
      "name": "Jobs.2016"
   },
   {
      "name": "Jobs.2017"
   },
   {
      "name": "Jobs.2018"
   },
   {
      "name": "Jobs.2019"
   },
   {
      "name": "Jobs.2020"
   },
   {
      "name": "Jobs.2021"
   },
   {
      "name": "Jobs.2022"
   },
   {
      "name": "Jobs.2023"
   },
   {
      "name": "Jobs.2024"
   },
   {
      "name": "Jobs.2025"
   },
   {
      "name": "Jobs.2026"
   },
   {
      "name": "Jobs.2027"
   },
   {
      "name": "Jobs.2028"
   },
   {
      "name": "Jobs.2029"
   },
   {
      "name": "Jobs.2030"
   },
   {
      "name": "Jobs.2031"
   },
   {
      "name": "Earnings.2001"
   },
   {
      "name": "Earnings.2002"
   },
   {
      "name": "Earnings.2003"
   },
   {
      "name": "Earnings.2004"
   },
   {
      "name": "Earnings.2005"
   },
   {
      "name": "Earnings.2006"
   },
   {
      "name": "Earnings.2007"
   },
   {
      "name": "Earnings.2008"
   },
   {
      "name": "Earnings.2009"
   },
   {
      "name": "Earnings.2010"
   },
   {
      "name": "Earnings.2011"
   },
   {
      "name": "Earnings.2012"
   },
   {
      "name": "Earnings.2013"
   },
   {
      "name": "Earnings.2014"
   },
   {
      "name": "Earnings.2015"
   },
   {
      "name": "Earnings.2016"
   },
   {
      "name": "Earnings.2017"
   },
   {
      "name": "Earnings.2018"
   },
   {
      "name": "Earnings.2019"
   },
   {
      "name": "Earnings.2020"
   },
   {
      "name": "Earnings.2021"
   },
   {
      "name": "Earnings.2022"
   },
   {
      "name": "Earnings.2023"
   },
   {
      "name": "EPW.2001"
   },
   {
      "name": "EPW.2002"
   },
   {
      "name": "EPW.2003"
   },
   {
      "name": "EPW.2004"
   },
   {
      "name": "EPW.2005"
   },
   {
      "name": "EPW.2006"
   },
   {
      "name": "EPW.2007"
   },
   {
      "name": "EPW.2008"
   },
   {
      "name": "EPW.2009"
   },
   {
      "name": "EPW.2010"
   },
   {
      "name": "EPW.2011"
   },
   {
      "name": "EPW.2012"
   },
   {
      "name": "EPW.2013"
   },
   {
      "name": "EPW.2014"
   },
   {
      "name": "EPW.2015"
   },
   {
      "name": "EPW.2016"
   },
   {
      "name": "EPW.2017"
   },
   {
      "name": "EPW.2018"
   },
   {
      "name": "EPW.2019"
   },
   {
      "name": "EPW.2020"
   },
   {
      "name": "EPW.2021"
   },
   {
      "name": "EPW.2022"
   },
   {
      "name": "EPW.2023"
   }
]
```
```json 2024.1
[
   {
      "name": "Jobs.2001"
   },
   {
      "name": "Jobs.2002"
   },
   {
      "name": "Jobs.2003"
   },
   {
      "name": "Jobs.2004"
   },
   {
      "name": "Jobs.2005"
   },
   {
      "name": "Jobs.2006"
   },
   {
      "name": "Jobs.2007"
   },
   {
      "name": "Jobs.2008"
   },
   {
      "name": "Jobs.2009"
   },
   {
      "name": "Jobs.2010"
   },
   {
      "name": "Jobs.2011"
   },
   {
      "name": "Jobs.2012"
   },
   {
      "name": "Jobs.2013"
   },
   {
      "name": "Jobs.2014"
   },
   {
      "name": "Jobs.2015"
   },
   {
      "name": "Jobs.2016"
   },
   {
      "name": "Jobs.2017"
   },
   {
      "name": "Jobs.2018"
   },
   {
      "name": "Jobs.2019"
   },
   {
      "name": "Jobs.2020"
   },
   {
      "name": "Jobs.2021"
   },
   {
      "name": "Jobs.2022"
   },
   {
      "name": "Jobs.2023"
   },
   {
      "name": "Jobs.2024"
   },
   {
      "name": "Jobs.2025"
   },
   {
      "name": "Jobs.2026"
   },
   {
      "name": "Jobs.2027"
   },
   {
      "name": "Jobs.2028"
   },
   {
      "name": "Jobs.2029"
   },
   {
      "name": "Jobs.2030"
   },
   {
      "name": "Jobs.2031"
   },
   {
      "name": "Earnings.2001"
   },
   {
      "name": "Earnings.2002"
   },
   {
      "name": "Earnings.2003"
   },
   {
      "name": "Earnings.2004"
   },
   {
      "name": "Earnings.2005"
   },
   {
      "name": "Earnings.2006"
   },
   {
      "name": "Earnings.2007"
   },
   {
      "name": "Earnings.2008"
   },
   {
      "name": "Earnings.2009"
   },
   {
      "name": "Earnings.2010"
   },
   {
      "name": "Earnings.2011"
   },
   {
      "name": "Earnings.2012"
   },
   {
      "name": "Earnings.2013"
   },
   {
      "name": "Earnings.2014"
   },
   {
      "name": "Earnings.2015"
   },
   {
      "name": "Earnings.2016"
   },
   {
      "name": "Earnings.2017"
   },
   {
      "name": "Earnings.2018"
   },
   {
      "name": "Earnings.2019"
   },
   {
      "name": "Earnings.2020"
   },
   {
      "name": "Earnings.2021"
   },
   {
      "name": "Earnings.2022"
   },
   {
      "name": "Earnings.2023"
   },
   {
      "name": "EPW.2001"
   },
   {
      "name": "EPW.2002"
   },
   {
      "name": "EPW.2003"
   },
   {
      "name": "EPW.2004"
   },
   {
      "name": "EPW.2005"
   },
   {
      "name": "EPW.2006"
   },
   {
      "name": "EPW.2007"
   },
   {
      "name": "EPW.2008"
   },
   {
      "name": "EPW.2009"
   },
   {
      "name": "EPW.2010"
   },
   {
      "name": "EPW.2011"
   },
   {
      "name": "EPW.2012"
   },
   {
      "name": "EPW.2013"
   },
   {
      "name": "EPW.2014"
   },
   {
      "name": "EPW.2015"
   },
   {
      "name": "EPW.2016"
   },
   {
      "name": "EPW.2017"
   },
   {
      "name": "EPW.2018"
   },
   {
      "name": "EPW.2019"
   },
   {
      "name": "EPW.2020"
   },
   {
      "name": "EPW.2021"
   },
   {
      "name": "EPW.2022"
   },
   {
      "name": "EPW.2023"
   }
]
```
```json 2023.3
[
   {
      "name": "Jobs.2001"
   },
   {
      "name": "Jobs.2002"
   },
   {
      "name": "Jobs.2003"
   },
   {
      "name": "Jobs.2004"
   },
   {
      "name": "Jobs.2005"
   },
   {
      "name": "Jobs.2006"
   },
   {
      "name": "Jobs.2007"
   },
   {
      "name": "Jobs.2008"
   },
   {
      "name": "Jobs.2009"
   },
   {
      "name": "Jobs.2010"
   },
   {
      "name": "Jobs.2011"
   },
   {
      "name": "Jobs.2012"
   },
   {
      "name": "Jobs.2013"
   },
   {
      "name": "Jobs.2014"
   },
   {
      "name": "Jobs.2015"
   },
   {
      "name": "Jobs.2016"
   },
   {
      "name": "Jobs.2017"
   },
   {
      "name": "Jobs.2018"
   },
   {
      "name": "Jobs.2019"
   },
   {
      "name": "Jobs.2020"
   },
   {
      "name": "Jobs.2021"
   },
   {
      "name": "Jobs.2022"
   },
   {
      "name": "Jobs.2023"
   },
   {
      "name": "Jobs.2024"
   },
   {
      "name": "Jobs.2025"
   },
   {
      "name": "Jobs.2026"
   },
   {
      "name": "Jobs.2027"
   },
   {
      "name": "Jobs.2028"
   },
   {
      "name": "Jobs.2029"
   },
   {
      "name": "Jobs.2030"
   },
   {
      "name": "Jobs.2031"
   },
   {
      "name": "Earnings.2001"
   },
   {
      "name": "Earnings.2002"
   },
   {
      "name": "Earnings.2003"
   },
   {
      "name": "Earnings.2004"
   },
   {
      "name": "Earnings.2005"
   },
   {
      "name": "Earnings.2006"
   },
   {
      "name": "Earnings.2007"
   },
   {
      "name": "Earnings.2008"
   },
   {
      "name": "Earnings.2009"
   },
   {
      "name": "Earnings.2010"
   },
   {
      "name": "Earnings.2011"
   },
   {
      "name": "Earnings.2012"
   },
   {
      "name": "Earnings.2013"
   },
   {
      "name": "Earnings.2014"
   },
   {
      "name": "Earnings.2015"
   },
   {
      "name": "Earnings.2016"
   },
   {
      "name": "Earnings.2017"
   },
   {
      "name": "Earnings.2018"
   },
   {
      "name": "Earnings.2019"
   },
   {
      "name": "Earnings.2020"
   },
   {
      "name": "Earnings.2021"
   },
   {
      "name": "Earnings.2022"
   },
   {
      "name": "EPW.2001"
   },
   {
      "name": "EPW.2002"
   },
   {
      "name": "EPW.2003"
   },
   {
      "name": "EPW.2004"
   },
   {
      "name": "EPW.2005"
   },
   {
      "name": "EPW.2006"
   },
   {
      "name": "EPW.2007"
   },
   {
      "name": "EPW.2008"
   },
   {
      "name": "EPW.2009"
   },
   {
      "name": "EPW.2010"
   },
   {
      "name": "EPW.2011"
   },
   {
      "name": "EPW.2012"
   },
   {
      "name": "EPW.2013"
   },
   {
      "name": "EPW.2014"
   },
   {
      "name": "EPW.2015"
   },
   {
      "name": "EPW.2016"
   },
   {
      "name": "EPW.2017"
   },
   {
      "name": "EPW.2018"
   },
   {
      "name": "EPW.2019"
   },
   {
      "name": "EPW.2020"
   },
   {
      "name": "EPW.2021"
   },
   {
      "name": "EPW.2022"
   }
]
```
```json 2023.1
[
   {
      "name": "Jobs.2001"
   },
   {
      "name": "Jobs.2002"
   },
   {
      "name": "Jobs.2003"
   },
   {
      "name": "Jobs.2004"
   },
   {
      "name": "Jobs.2005"
   },
   {
      "name": "Jobs.2006"
   },
   {
      "name": "Jobs.2007"
   },
   {
      "name": "Jobs.2008"
   },
   {
      "name": "Jobs.2009"
   },
   {
      "name": "Jobs.2010"
   },
   {
      "name": "Jobs.2011"
   },
   {
      "name": "Jobs.2012"
   },
   {
      "name": "Jobs.2013"
   },
   {
      "name": "Jobs.2014"
   },
   {
      "name": "Jobs.2015"
   },
   {
      "name": "Jobs.2016"
   },
   {
      "name": "Jobs.2017"
   },
   {
      "name": "Jobs.2018"
   },
   {
      "name": "Jobs.2019"
   },
   {
      "name": "Jobs.2020"
   },
   {
      "name": "Jobs.2021"
   },
   {
      "name": "Jobs.2022"
   },
   {
      "name": "Jobs.2023"
   },
   {
      "name": "Jobs.2024"
   },
   {
      "name": "Jobs.2025"
   },
   {
      "name": "Jobs.2026"
   },
   {
      "name": "Jobs.2027"
   },
   {
      "name": "Jobs.2028"
   },
   {
      "name": "Jobs.2029"
   },
   {
      "name": "Jobs.2030"
   },
   {
      "name": "Jobs.2031"
   },
   {
      "name": "Jobs.2032"
   },
   {
      "name": "Jobs.2033"
   },
   {
      "name": "Earnings.2001"
   },
   {
      "name": "Earnings.2002"
   },
   {
      "name": "Earnings.2003"
   },
   {
      "name": "Earnings.2004"
   },
   {
      "name": "Earnings.2005"
   },
   {
      "name": "Earnings.2006"
   },
   {
      "name": "Earnings.2007"
   },
   {
      "name": "Earnings.2008"
   },
   {
      "name": "Earnings.2009"
   },
   {
      "name": "Earnings.2010"
   },
   {
      "name": "Earnings.2011"
   },
   {
      "name": "Earnings.2012"
   },
   {
      "name": "Earnings.2013"
   },
   {
      "name": "Earnings.2014"
   },
   {
      "name": "Earnings.2015"
   },
   {
      "name": "Earnings.2016"
   },
   {
      "name": "Earnings.2017"
   },
   {
      "name": "Earnings.2018"
   },
   {
      "name": "Earnings.2019"
   },
   {
      "name": "Earnings.2020"
   },
   {
      "name": "Earnings.2021"
   },
   {
      "name": "Earnings.2022"
   },
   {
      "name": "Earnings.2023"
   },
   {
      "name": "Earnings.2024"
   },
   {
      "name": "EPW.2001"
   },
   {
      "name": "EPW.2002"
   },
   {
      "name": "EPW.2003"
   },
   {
      "name": "EPW.2004"
   },
   {
      "name": "EPW.2005"
   },
   {
      "name": "EPW.2006"
   },
   {
      "name": "EPW.2007"
   },
   {
      "name": "EPW.2008"
   },
   {
      "name": "EPW.2009"
   },
   {
      "name": "EPW.2010"
   },
   {
      "name": "EPW.2011"
   },
   {
      "name": "EPW.2012"
   },
   {
      "name": "EPW.2013"
   },
   {
      "name": "EPW.2014"
   },
   {
      "name": "EPW.2015"
   },
   {
      "name": "EPW.2016"
   },
   {
      "name": "EPW.2017"
   },
   {
      "name": "EPW.2018"
   },
   {
      "name": "EPW.2019"
   },
   {
      "name": "EPW.2020"
   },
   {
      "name": "EPW.2021"
   },
   {
      "name": "EPW.2022"
   },
   {
      "name": "EPW.2023"
   },
   {
      "name": "EPW.2024"
   }
]
```

<br />

<br />

Attributes

<br />

## Schema

| Fields       | Snowflake | BigQuery   | Databricks | Description                                                                                                                                    |
| :----------- | :-------- | :--------- | :--------- | :--------------------------------------------------------------------------------------------------------------------------------------------- |
| AREAID       | VARCHAR   | STRING     | STRING     | ID of the geographic region.                                                                                                                   |
| AREAID_NAME  | VARCHAR   | STRING     | STRING     | Name of the geographic region.                                                                                                                 |
| AREAID_TYPE  | VARCHAR   | STRING     | STRING     | Geographic area type.                                                                                                                          |
| CLASSID      | VARCHAR   | STRING     | STRING     | ID of the class of worker.                                                                                                                     |
| CLASSID_NAME | VARCHAR   | STRING     | STRING     | Name of the class of worker.                                                                                                                   |
| EARN         | FLOAT     | FLOAT      | DOUBLE     | Total earnings for the industry (wages + supplements). This figure is also for the whole industry, not for the average worker in the industry. |
| EMP          | FLOAT     | FLOAT      | DOUBLE     | The number of occupied positions.                                                                                                              |
| INDID        | VARCHAR   | STRING     | STRING     | NAICS code.                                                                                                                                    |
| INDID_NAME   | VARCHAR   | STRING     | STRING     | NAICS name.                                                                                                                                    |
| YEAR         | NUMBER    | BIGNUMERIC | DECIMAL    | Year of data.                                                                                                                                  |

<Callout icon="🚧" theme="warn">
  Above schema is for demo purpose, during production respective schema will be provided for each dataset.
</Callout>

<br />
