---
layout: default
title: Tableau Web Data Connector
parent: Tableau
nav_order: 1
custom_css:
- tooltips
custom_js:
- latex
---

# Tableau Web Data Connector
{: .no_toc }

<br>

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

<br>

### Connectors

<a href="https://tableau.github.io/webdataconnector/" target="\_blank">Tableau Web Data Connectors</a> enable web data source connections, specifically JSON data sources.  The example discussed herein reads JSON data files hosted by GitHub.

#### Example

Imagine a task wherein we have to illustrate the daily

<ul style="margin-left: 35px">
  <li style="margin-bottom: 10px">$\small{deaths_{c}/100K}$ $vs.$ $\small{positives_{c}/100K}$</li>
  <li>$\small{positives_{c}/100K}$ $vs.$ $\small{tests_{c}/100K}$</li>
</ul>

wherein

<div style="margin-left: 35px">$c$: cumulative</div>

in relation to <span class="tooltip">SARS-CoV-2<span class="tooltiptext">Severe Acute Respiratory Syndrome Coronavirus 2</span></span> infections in the states of the U.S.A..  [In well managed settings, the time varying gradients of the ensuing curves, and the forecasts of such curves, could be quite helpful.]

<br>

We might opt for 2 graph data sources

<ul style="margin-left: 35px">
  <li><a href="https://raw.githubusercontent.com/briefings/sars/master/fundamentals/atlantic/warehouse/capita.json" target="\_blank">capita.json</a> A source that summarises each day's rate values per state.</li>
  <li><a href="https://raw.githubusercontent.com/briefings/sars/master/fundamentals/atlantic/warehouse/gazetteer.json">gazetteer.json</a> a gazetteer file, i.e., a file that summarises geographic, etc., facts of each state.</li>
</ul>

In this example, each data source is read  by its own Tableau Web Data Connector.  In brief.  The data source [capita.json](https://raw.githubusercontent.com/briefings/sars/master/fundamentals/atlantic/warehouse/capita.json) is read by a connector named [capita.html](https://github.com/miscellane/tableau/blob/master/pages/capita.html), which reads the source via script file [capita.js](https://github.com/miscellane/tableau/blob/master/pages/gazetteer.html); the schema of capita.json is detailed in capita.js.  And,  data source [gazetteer.json](https://raw.githubusercontent.com/briefings/sars/master/fundamentals/atlantic/warehouse/gazetteer.json) is read by a connector named [gazetteer.html](https://github.com/miscellane/tableau/blob/master/pages/gazetteer.html), which reads the source via script file [gazetteer.js](https://github.com/miscellane/tableau/blob/master/assets/js/gazetteer.js); the schema of gazetteer.json is detailed in gazetteer.js.  

The data sets are joined, via a common key, prior to drawing the graphs illustrated below.

<div style="margin-left: 70px">
  <div class='tableauPlaceholder' id='viz1605126180958' style='position: relative'>
    <noscript><a href='#'><img alt=' ' src='https://public.tableau.com/static/images/ca/capita_16051250435120/capita_twb/1_rss.png' style='border: none' /></a>
    </noscript>
    <object class='tableauViz'  style='display:none;'>
      <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' />
      <param name='embed_code_version' value='3' />
      <param name='site_root' value='' />
      <param name='name' value='capita_16051250435120/capita_twb' />
      <param name='tabs' value='no' />
      <param name='toolbar' value='yes' />
      <param name='static_image' value='https://public.tableau.com/static/images/ca/capita_16051250435120/capita_twb/1.png' />
      <param name='animate_transition' value='yes' />
      <param name='display_static_image' value='yes' />
      <param name='display_spinner' value='yes' />
      <param name='display_overlay' value='yes' />
      <param name='display_count' value='yes' />
      <param name='language' value='en-GB' />
      <param name='filter' value='publish=yes' />
    </object>
  </div>
  <script type='text/javascript'>
      var divElement = document.getElementById('viz1605126180958');
      var vizElement = divElement.getElementsByTagName('object')[0];
      vizElement.style.width='550px';vizElement.style.height='627px';
      var scriptElement = document.createElement('script');
      scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';
      vizElement.parentNode.insertBefore(scriptElement, vizElement);
  </script>
</div>

<br>
<br>

### Limitations of Tableau Web Data Connectors

Alas, the tools required for automatically updating Tableau graphs based on Tableau web data connector feeds are only available via Tableau Online or Tableau Server; Tableau Public projects can't be updated automatically.
