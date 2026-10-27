<div align="center">

<img src="./images/cover.png" alt="M02 AlienVault OTX and YARA" width="100%" />

<br><br>

<h1>M02 — AlienVault OTX and YARA</h1>
<h3>The threat intelligence lifecycle from collection to a custom YARA indicator</h3>

<br>

<img src="https://img.shields.io/badge/TYPE-INTELLIGENCE%20LIFECYCLE-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />
<img src="https://img.shields.io/badge/TASKS-4-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />
<img src="https://img.shields.io/badge/TOOLS-OTX%20%7C%20YARA-0d1117?style=for-the-badge&labelColor=0d1117&color=00b4d8" />

<br><br>

<a href="#overview"><b>Overview</b></a> &nbsp;·&nbsp;
<a href="#tasks-and-results"><b>Tasks</b></a> &nbsp;·&nbsp;
<a href="#evidence"><b>Evidence</b></a> &nbsp;·&nbsp;
<a href="#full-report"><b>Report</b></a>

</div>

<br>

---

## Overview

A four-task lab that walks the full lifecycle on AlienVault OTX: collecting indicators from community pulses, scanning an endpoint with the OTX agent, writing a custom YARA indicator for a Linux ELF sample from MalwareBazaar, and reviewing the sharing options. The lab ran on a Windows 10 virtual machine with Windows Defender disabled so the agent and samples could run without interference.

<br>

## Tasks and Results

<table>
<tr><th>Task</th><th>Activity</th><th>Result</th></tr>
<tr><td><b>1</b></td><td>IoC data collection from subscribed pulses</td><td>Pulse <i>Silent Crypto Wallet Takeover</i> reviewed: 4 IoCs (3 phishing URLs and 1 YARA rule) and 18+ ATT&amp;CK techniques</td></tr>
<tr><td><b>2</b></td><td>Threat analysis with OTX Endpoint Security</td><td>Agent installed through PowerShell; endpoint registered on Windows 10.0.17763 with no matches</td></tr>
<tr><td><b>3</b></td><td>Custom YARA indicator for an ELF sample</td><td>Rule <code>MAL_Linux_ELF_Hash_Exact</code> matches the exact SHA-256; the OTX test returned no false positives; role <code>file_scanning</code>, no expiration</td></tr>
<tr><td><b>4</b></td><td>Sharing and dissemination</td><td>Pulse <i>Suspicious Linux ELF Executable Detection (YARA)</i> published as TLP:WHITE (private); sharing actions reviewed: subscribe, download CSV, OpenIOC and STIX, embed, clone, suggest edit</td></tr>
</table>

<br>

## Evidence

<p align="center">
  <img src="./images/otx-endpoint-registered.png" alt="OTX endpoint registered" width="800"/><br/>
  <sub>Task 2: endpoint registered in OTX Endpoint Security</sub>
</p>

<p align="center">
  <img src="./images/yara-rule-editor.png" alt="YARA rule editor" width="800"/><br/>
  <sub>Task 3: YARA rule with SHA-256 condition and the Test Scan Rule button</sub>
</p>

<p align="center">
  <img src="./images/yara-no-false-positives.png" alt="YARA no false positives" width="800"/><br/>
  <sub>Task 3: OTX reports no false positives for the rule</sub>
</p>

<p align="center">
  <img src="./images/pulse-published.png" alt="Published pulse" width="800"/><br/>
  <sub>Task 3: published pulse header with TLP:WHITE and tags</sub>
</p>

<p align="center">
  <img src="./images/community-pulse-iocs.png" alt="Community pulse IoCs" width="800"/><br/>
  <sub>Task 4: IoC details of a public community pulse</sub>
</p>

<br>

## Tools

<code>AlienVault OTX</code> <code>OTX Endpoint Security</code> <code>YARA</code> <code>MalwareBazaar</code> <code>PowerShell</code>

<br>

## Full Report

📄 **[OTX-and-YARA.pdf](./OTX-and-YARA.pdf)**: all four tasks with every step and figure.

<br>

<div align="center">

⬅ <a href="../README.md"><b>Back to Main Repository</b></a>

</div>
