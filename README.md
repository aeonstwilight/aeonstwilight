### Hi, I'm Ryan 👋

Detection engineer and SOC analyst with 6+ years in security operations and 10 years in IT. I write detections, investigate incidents and hunt threats across Windows, Active Directory and cloud (AWS and Azure) environments.

I like detections I can prove: tested against real attack data, run on a real engine, and shipped with the triage steps an analyst needs at 2 a.m.

- 🔍 **Focus:** detection engineering, incident response, threat hunting, ATT&CK-aligned coverage
- 🛠️ **Day to day:** Splunk SPL, KQL (Microsoft Sentinel / Defender XDR), Elastic, Sigma, Sysmon and Windows event logs, AWS CloudTrail, CrowdStrike, Trend Micro DSM, SentinelOne, Carbon Black, Qualys, Tenable Nessus
- 🐍 **Scripting:** Python and PowerShell, plus LLM-assisted detection engineering
- 📜 **Certification:** ISO/IEC 27001 Lead Auditor
- 🎓 **Education:** BS, Information & Computer Security, Davenport University
- 🌐 **Write-ups:** [rwilliams.dev](https://rwilliams.dev)
- 📫 **Reach me:** [LinkedIn](https://www.linkedin.com/in/williams-ryan/)

### Open source contributions

**[SigmaHQ/pySigma-backend-elasticsearch](https://github.com/SigmaHQ/pySigma-backend-elasticsearch)**, the converter behind `sigma convert` for Elasticsearch:
- Fixed ES|QL `LIKE` escaping, so rules matching Windows paths no longer produce queries Elasticsearch rejects ([#238](https://github.com/SigmaHQ/pySigma-backend-elasticsearch/pull/238), merged)
- Translated Sigma regexes for Lucene's whole-value matching: exact matches went from 25 to 211 of 215 SigmaHQ regex conditions, tested on Elasticsearch ([#241](https://github.com/SigmaHQ/pySigma-backend-elasticsearch/pull/241), merged)


### Projects

[unopened](https://github.com/aeonstwilight/unopened): static malware triage for SOC analysts. Takes a suspicious file and writes one plain-language report: what it is, what it can do, which indicators to hunt for, and how confident the verdict is, without ever running or opening the file. Covers Windows programs, Office macros, RTF, PDFs, shortcuts, scripts, HTML and SVG smuggling, emails and archives, defangs every indicator, and writes hunt queries for Splunk, Microsoft Sentinel and Elastic. Verdicts come from documented rules, not a model, and every report lists what was not checked. Validated on real malware in an isolated VM (0 malicious verdicts on 347 benign files), with every miss [published](https://github.com/aeonstwilight/unopened/blob/main/docs/validation.md).

**[security-automation-scripts](https://github.com/aeonstwilight/security-automation-scripts)**: detections and SOC scripts. Each detection is one file with the logic, queries for Splunk, Microsoft Sentinel and Elastic, false positives, blind spots, how to validate it and how to respond. Covers Windows and Active Directory (ransomware precursors, lateral movement, WMI, Office abuse) and AWS (logging disabled, root activity, console login without MFA, credentials created for another user, resources opened to the internet), plus a Windows triage script.
