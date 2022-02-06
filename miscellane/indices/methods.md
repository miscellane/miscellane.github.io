---
layout: default
title: Methods
parent: Indices
nav_order: 1
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

<h2>Research Strategy</h2>

<h3>Illustration</h3>

<br>

<br>

<h3>Validity</h3>

<table style="width: 55%; font-size: 65%; text-align: left;">
    <colgroup>
        <col span="1" style="width: 10%;">
        <col span="1" style="width: 20%;">
        <col span="1" style="width: 25%;">
    </colgroup>
    <thead>
        <tr><th>validity</th><th>focus</th><th>threats & mitigations of</th></tr>
    </thead>
    <tr>
        <td><a href="https://conjointly.com/kb/external-validity/" target="_blank">External</a></td>
        <td>Sampling.  <i>The degree to which a study's conclusions can be generalised to the population.</i></td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://conjointly.com/kb/construct-validity/" target="_blank">Construct</a></td>
        <td>Measurement.  Is the operational setting, or are the measures, in line with the hypothesis construct?</td>
        <td></td>
    </tr>
    <tr>
        <td><a href="https://conjointly.com/kb/internal-validity/" target="_blank">Internal</a></td>
        <td>Design.  The degree to which a cause & effect relationship can be discerned between a set of factors and outcome variables</td>
        <td>Not applicable</td>
    </tr>
    <tr>
        <td><a href="https://conjointly.com/kb/conclusion-validity/" target="_blank">Conclusion</a></td>
        <td>Analysis.  <i>"... the degree to which conclusions we reach about relationships in our data are reasonable."</i></td>
        <td></td>
    </tr>
</table>

<br>

<h2>Data</h2>

**Focus:** 
> England, United Kingdom

**Unit:** 
> Lower Tier Local Authority

<br>

<h3>Projection Variables</h3>

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

<h4>Mortality Rates</h4>

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

<br>

<h4>DALY, YLL, YLD</h4>

<br>

<h3>Potential Prognostic Factors</h3>

Thus far:

* The ONS Indices of Multiple Deprivation
* [Access to Healthy Assets & Hazards (AHAH)](https://data.cdrc.ac.uk/dataset/access-healthy-assets-hazards-ahah)
* Food Desert Score


<h4>Indices of Multiple Deprivation (IMD)</h4>

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
        <td>Education, Skills and Training Rank [Children and Young People Sub-domain Rank, Adult Skills Sub-domain Rank]; Barriers to Housing and Services Rank [Geographical Barriers Sub-domain Rank, Wider Barriers Sub-domain Rank]; Living Environment Rank [Indoors Sub-domain Rank, Outdoors Sub-domain Rank]</td>
    </tr>
    <tr>
        <td>ranking note</td>
        <td>1 is most deprived</td>
    </tr>
</table>
