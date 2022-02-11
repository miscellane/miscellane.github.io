---
layout: default
title: Methods
parent: Indices
nav_order: 2
custom_css:
- tooltips
custom_js:
- latex
---

# Methods
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

<br>

**Focus:** 
> England, United Kingdom

**Unit:** 
> Lower Tier Local Authority

<br>

## Dependent Variables

The dependent variable will be annual prevalence rate.

<table style="width: 55%; font-size: 65%; text-align: left;">
    <colgroup>
        <col span="1" style="width: 10%;">
        <col span="1" style="width: 45%;">
    </colgroup>
    <thead>
        <tr><th>item</th><th>value/element</th></tr>
    </thead>
    <tr>
        <td>chronic disease code</td>
        <td>International Classification of Diseases,Tenth Revision (ICD-10)</td>
    </tr>
    <tr>
        <td>chronic disease name</td>
        <td>Malignant neoplasms<br>Diabetes mellitus<br>Obesity and other hyperalimentation<br>Mental and 
            behavioural disorders due to psychoactive substance use<br>Hypertensive diseases<br>Ischaemic heart 
            diseases<br>Chronic lower respiratory diseases<br>Diseases of liver<br>Renal failure</td>
    </tr>
    <tr>
        <td>catchment area</td>
        <td>lower tier local authority or general practice</td>
    </tr>
    <tr>
        <td>period</td>
        <td>2004, ..., 2020</td>
    </tr>
    <tr>
        <td>sex</td>
        <td>sex</td>
    </tr>
    <tr>
        <td>age group</td>
        <td><i>0 - 4, 5 - 9, 10 - 14, ..., 85 - 89, 90+</i></td>
    </tr>
    <tr>
        <td>measures</td>
        <td>number of diagnosed individuals</td>
    </tr>
    <tr>
        <td></td>
        <td>population</td>
    </tr>
</table>

<br>
<br>


## Independent Variables


Potentially, and per lower tier local authority:

* age & sex adjusted mortality rates [per 100,000 of population]
* disease burden, i.e., either 
  * disability-adjusted life years (DALYs), 
  * years of life lost due to premature mortality ([YLLs](https://www.who.int/data/gho/indicator-metadata-registry/imr-details/4427)),
  * years of life lost due to time lived in states of less than full health / years of healthy life lost due to disability 
    ([YLDs](https://www.who.int/data/gho/indicator-metadata-registry/imr-details/4429))
  &nbsp; &nbsp; In each case, per 100,000 of population
* disease treatment & management cost per 100,000 of population    

<br>

#### **Mortality Rates**

<br>

Nomis provides the LTLA death numbers per chronic disease per year.  Hence, the project has to calculate each year's age & sex adjusted mortality rates per chronic disease per year.

<p style="margin-left:35px">
$r_{_{l}} = \sum_{_{l}} r_{_{ag, s, l}}$
</p>

<p style="margin-left:35px">
$r_{_{ag, s, l}} = 100000 \times \Large{ \frac{d_{_{ag, s, l}}}{p_{_{ag, s, l}}} }$
</p>

<br>

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

<br>

#### **DALY, YLL, YLD**

<br>
<br>

<br>
<br>

#### **Indices of Multiple Deprivation (IMD)**


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
        <td>IMD</td>
    </tr>
    <tr>
        <td>granularity/by</td>
        <td>LSOA</td>
    </tr>
    <tr>
        <td>latest</td>
        <td>2019</td>
    </tr>
    <tr>
        <td>domains</td>
        <td>Income Rank (22.5%); Employment Rank (22.5%); Education, Skills and Training Rank (13.5%); Health Deprivation and Disability Rank (13.5%); Crime Rank (9.3%); Barriers to Housing and Services Rank (9.3%); Living Environment Rank (9.3%)</td>
    </tr>
    <tr>
        <td>rank note</td>
        <td>1 is most deprived</td>
    </tr>
    <tr>
        <td>comment</td>
        <td>The values within the parentheses are the ONS weights for the overarching IMD</td>
    </tr>
</table>

<br>

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
        <td>IMD</td>
    </tr>
    <tr>
        <td>granularity/by</td>
        <td>LSOA</td>
    </tr>
    <tr>
        <td>latest</td>
        <td>2019</td>
    </tr>
    <tr>
        <td>sub-domains</td>
        <td>Education, Skills and Training Rank [Children and Young People Sub-domain Rank, Adult Skills Sub-domain Rank]; Barriers to Housing and Services Rank [Geographical Barriers Sub-domain Rank, Wider Barriers Sub-domain Rank]; Living Environment Rank [Indoors Sub-domain Rank, Outdoors Sub-domain Rank]</td>
    </tr>
    <tr>
        <td>rank note</td>
        <td>1 is most deprived</td>
    </tr>
</table>
