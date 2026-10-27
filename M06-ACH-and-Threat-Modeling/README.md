<div align="center">

<img src="./images/cover.png" alt="M06 ACH and Threat Modeling" width="100%" />

<br><br>

<h1>M06 — ACH and Threat Modeling</h1>
<h3>Competing hypotheses on a suspected supply chain patch and STRIDE threat modeling</h3>

<br>

<img src="https://img.shields.io/badge/TYPE-STRUCTURED%20ANALYSIS-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />
<img src="https://img.shields.io/badge/LABS-2-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />
<img src="https://img.shields.io/badge/TOOLS-PARC%20ACH%20%7C%20MS%20TMT-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />

<br><br>

<a href="#overview"><b>Overview</b></a> &nbsp;·&nbsp;
<a href="#tasks-and-results"><b>Results</b></a> &nbsp;·&nbsp;
<a href="#evidence"><b>Evidence</b></a> &nbsp;·&nbsp;
<a href="#full-report"><b>Report</b></a>

</div>

<br>

---

## Overview

Two structured analytic techniques. In the first, PARC ACH 2.0.5 is used to weigh two explanations for suspicious database activity after a vendor security patch. In the second, Microsoft Threat Modeling Tool 2016 is used to build a small request and response model from scratch, then to run a prebuilt WebRequestModel through the STRIDE knowledge base and generate a full report.

<br>

## Tasks and Results

<table>
<tr><th>Lab</th><th>Activity</th><th>Result</th></tr>
<tr><td><b>ACH</b></td><td>Hypotheses: H1 the EHR vendor was compromised and a malicious patch was deployed; H2 the patch is legitimate and database permissions are too broad</td><td>Two evidence items rated: queries aimed at payment and insurance data, and identical patterns at three other hospitals within 24 hours</td></tr>
<tr><td><b>ACH</b></td><td>Weighted inconsistency per hypothesis</td><td>H1 scored 1.414 and H2 scored 3.535; the lower score marks H1, the malicious patch, as the better supported explanation</td></tr>
<tr><td><b>Threat model</b></td><td>Built a Human User to External Web Application model with HTTP Request and Response flows</td><td>Basic request and response lifecycle modeled; flows named for traceable threats</td></tr>
<tr><td><b>Threat model</b></td><td>WebRequestModel: User, Web Application, Web Server and Cloud Storage; template SDL TM Knowledge Base (Core) v4.1.0.9</td><td>Full report generated with 44 threats: 38 Not Started, 4 Needs Investigation, 2 Mitigation Implemented</td></tr>
</table>

<br>

## Evidence

<p align="center">
  <img src="./images/ach-matrix-ratings.png" alt="ACH matrix ratings" width="800"/><br/>
  <sub>ACH: matrix with evidence ratings applied to both hypotheses</sub>
</p>

<p align="center">
  <img src="./images/ach-inconsistency-chart.png" alt="ACH inconsistency chart" width="800"/><br/>
  <sub>ACH: inconsistencies per hypothesis, H1 lower than H2</sub>
</p>

<p align="center">
  <img src="./images/threat-model-http-flow.png" alt="Basic threat model" width="800"/><br/>
  <sub>Threat model: completed HTTP Request and Response model</sub>
</p>

<p align="center">
  <img src="./images/webrequestmodel-dfd.png" alt="WebRequestModel diagram" width="800"/><br/>
  <sub>Threat model: WebRequestModel data flow diagram</sub>
</p>

<p align="center">
  <img src="./images/threat-report-summary.png" alt="Threat report summary" width="800"/><br/>
  <sub>Threat model: report summary showing 44 threats by state</sub>
</p>

<br>

## Tools

<code>PARC ACH 2.0.5</code> <code>Microsoft Threat Modeling Tool 2016</code> <code>STRIDE</code>

<br>

## Full Report

📄 **[ACH-and-Threat-Modeling.pdf](./ACH-and-Threat-Modeling.pdf)**: the ACH and threat modeling labs with every step and figure.

<br>

<div align="center">

⬅ <a href="../README.md"><b>Back to Main Repository</b></a>

</div>
