<div align="center">

<img src="./images/cover.png" alt="M08 Healthcare Breach Analysis" width="100%" />

<br><br>

<h1>M08 — Healthcare Breach Analysis (Zoho, Tableau, Qlik)</h1>
<h3>One breach dataset, three analytics platforms</h3>

<br>

<img src="https://img.shields.io/badge/TYPE-DATA%20ANALYTICS-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />
<img src="https://img.shields.io/badge/PLATFORMS-3-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />
<img src="https://img.shields.io/badge/RECORDS-1%2C151-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />

<br><br>

<a href="#overview"><b>Overview</b></a> &nbsp;·&nbsp;
<a href="#tasks-and-results"><b>Results</b></a> &nbsp;·&nbsp;
<a href="#evidence"><b>Evidence</b></a> &nbsp;·&nbsp;
<a href="#full-report"><b>Reports</b></a>

</div>

<br>

---

## Overview

The HHS Cyber Security Breaches dataset (1,151 records of healthcare breaches reported to the US Department of Health and Human Services, 10 columns) is analysed in Zoho Analytics, Tableau Desktop 2018.1 and Qlik Cloud Analytics. The aim is to show how bulk data is ingested, joined, filtered and visualised to expose patterns that raw tables hide.

<br>

## Tasks and Results

<table>
<tr><th>Tool</th><th>Activity</th><th>Result</th></tr>
<tr><td><b>Zoho Analytics</b></td><td>Imported the CSV into a workspace; built line and bubble charts by entity type, breach type and breach location</td><td>All 1,151 rows and 10 columns imported; Healthcare Providers show the highest impact, with Hacking/IT Incident peaking above 9 million individuals</td></tr>
<tr><td><b>Tableau</b></td><td>Joined <code>HHSCyberSecurityBreaches.csv</code> and <code>breaches.csv</code> (inner join on F1); filtered Individuals Affected to 1,500 to 2,000</td><td>Filter returned 90 rows</td></tr>
<tr><td><b>Tableau</b></td><td>Packed bubbles and stacked bar charts by state</td><td>Total of 37,773,276 individuals affected; Tennessee the tallest bar, followed by Indiana and Illinois, New York and Texas</td></tr>
<tr><td><b>Qlik Cloud</b></td><td>Created the <i>Healthcare_Breach_Analysis</i> app with a KPI and a map on the sheet <i>Total Individuals Affected</i></td><td>About 1,150 records loaded; KPI count 1.15k; column headers were not detected, so fields appear as <code>@1</code>, <code>@10</code></td></tr>
</table>

<br>

## Evidence

<p align="center">
  <img src="./images/zoho-import-summary.png" alt="Zoho import summary" width="800"/><br/>
  <sub>Zoho: import summary with 1,151 rows and 10 columns</sub>
</p>

<p align="center">
  <img src="./images/zoho-line-chart.png" alt="Zoho line chart" width="800"/><br/>
  <sub>Zoho: individuals affected by entity type and breach type</sub>
</p>

<p align="center">
  <img src="./images/zoho-bubble-chart.png" alt="Zoho bubble chart" width="800"/><br/>
  <sub>Zoho: multi-dimensional bubble chart with tooltip</sub>
</p>

<p align="center">
  <img src="./images/tableau-inner-join.png" alt="Tableau inner join" width="800"/><br/>
  <sub>Tableau: inner join of the two datasets on F1</sub>
</p>

<p align="center">
  <img src="./images/tableau-packed-bubbles.png" alt="Tableau packed bubbles" width="800"/><br/>
  <sub>Tableau: packed bubbles of individuals affected by state</sub>
</p>

<p align="center">
  <img src="./images/tableau-stacked-bar.png" alt="Tableau stacked bar" width="800"/><br/>
  <sub>Tableau: stacked bar chart, Tennessee tallest</sub>
</p>

<p align="center">
  <img src="./images/qlik-kpi-map-sheet.png" alt="Qlik KPI and map sheet" width="800"/><br/>
  <sub>Qlik: sheet with KPI count and map</sub>
</p>

<br>

## Tools

<code>Zoho Analytics</code> <code>Tableau Desktop 2018.1</code> <code>Qlik Cloud Analytics</code>

<br>

## Full Reports

📄 **[Tableau-and-Qlik.pdf](./Tableau-and-Qlik.pdf)**: the Tableau and Qlik parts with every step and figure.

📄 **[ACH-and-Threat-Modeling.pdf](../M06-ACH-and-Threat-Modeling/ACH-and-Threat-Modeling.pdf)**: the Zoho Analytics part is Lab 3 of this report.

<br>

<div align="center">

⬅ <a href="../README.md"><b>Back to Main Repository</b></a>

</div>
