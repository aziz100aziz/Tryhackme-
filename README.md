# Report: Phishing Unfolding — TryHackMe

This repository contains a detailed report documenting the analysis of the **Phishing Unfolding** room from TryHackMe. The goal of this work is to investigate how a phishing campaign unfolds, identify Indicators of Compromise (IOCs), and provide insights and recommendations for detection and prevention.

---

## Repository Contents
- `report.pdf` — The full report (analysis, screenshots, commands, outputs, findings, and recommendations).
- (Optional) `screenshots/` — Screenshots referenced in the report.
- (Optional) `ioc.txt` — Extracted Indicators of Compromise (URLs, IPs, domains).

---

## What Was Done
- Investigated and analyzed the phishing scenario from TryHackMe.
- Examined suspicious URLs and traced redirections.
- Reviewed landing pages and source code (HTML/JS) to detect phishing techniques.
- Collected Indicators of Compromise (IOCs) such as URLs, domains, and IP addresses.
- Documented methodology, findings, and recommendations in `report.pdf`.

---

## How to Open the Report
1. Open this repository on GitHub.
2. Click on `report.pdf` to view it directly in GitHub, or download it locally.
3. Use any PDF reader (browser, Adobe Reader, etc.) to view the file.

---

## General Steps to Reproduce the Analysis
> Perform these steps only in a **safe, isolated environment** (e.g., a VM).

1. Set up an isolated lab environment (virtual machine).
2. Obtain the suspicious URL/sample from the TryHackMe room.
3. Use tools such as `curl -I <url>`, `wget`, or HTTP header analysis to follow redirections.
4. Inspect the page source (`view-source:`) for forms, hidden scripts, or suspicious external calls.
5. Collect domains/IPs and check them with WHOIS or threat intelligence tools.
6. Document findings, take screenshots, and compile IOCs.

---

## Key Findings (Summary)
- The phishing technique relied on imitating a legitimate login page and/or using redirection through intermediary domains.
- Shortened or intermediate links were used to hide the real malicious source.
- Main recommendation: strengthen user awareness, apply mail filtering, and verify links in a sandbox environment before interaction.

---

## Recommendations
- Implement URL sandboxing in the email gateway.
- Configure filtering rules to block malicious or suspicious domains.
- Provide security awareness training for users to identify phishing attempts.
- Maintain and share updated lists of IOCs with security teams.

---

## Credits & License
- Author: **[aziz albatol]**  
- You may add a license for this repository (e.g., `MIT`) by including a `LICENSE` file.

---

## Contact
For questions, feedback, or clarifications, please open an Issue in this repository or reach out through the contact details provided in my profile.

---
