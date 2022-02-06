---
layout: default
title: Background Research
parent: Indices
nav_order: 1
custom_css:
- tooltips
custom_js:
- latex
---

# Background Research
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---


## Data

**Focus:** 
> England, United Kingdom

**Unit:** 
> Lower Tier Local Authority


### Projection Variables

Potentially, and per lower tier local authority:

* age & sex adjusted mortality rates [per 100,000 of population]
* disease burden, i.e., either 
  * disability-adjusted life years (DALYs), 
  * years of life lost due to premature mortality ([YLLs](https://www.who.int/data/gho/indicator-metadata-registry/imr-details/4427)),
  * years of life lost due to time lived in states of less than full health / years of healthy life lost due to disability 
    ([YLDs](https://www.who.int/data/gho/indicator-metadata-registry/imr-details/4429))
  &nbsp; &nbsp; In each case, per 100,000 of population
* disease treatment & management cost per 100,000 of population    

#### Mortality Rates

The age & sex adjusted mortality rates

$r_{l} = \sum_{l} r_{ag, s, l}$

<table style="width: 55%; font-size: 65%; text-align: left;">
    <colgroup>
        <col span="1" style="width: 10%;">
        <col span="1" style="width: 45%;">
    </colgroup>
    <thead>
        <tr><th></th><th>description</th></tr>
    </thead>
    <tr>
        <td>variable</td>
        <td>death</td>
    </tr>
    <tr>
        <td>granularity/by</td>
        <td>age group, sex, LTLA</td>
    </tr>
    <tr>
        <td>period</td>
        <td>2013, ..., 2020</td>
    </tr>
    <tr>
        <td>diseases</td>
        <td>C00-C97 Malignant neoplasms, E10-E14 Diabetes mellitus, E65-E68 Obesity and other hyperalimentation, F10-F19 Mental and 
            behavioural disorders due to psychoactive substance use, I10-I15 Hypertensive diseases, I20-I25 Ischaemic heart 
            diseases, J40-J47 Chronic lower respiratory diseases, K70-K77 Diseases of liver, N17-N19 Renal failure</td>
    </tr>
</table>
