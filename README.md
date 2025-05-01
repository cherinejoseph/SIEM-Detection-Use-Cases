# 📊 SIEM Detection Use Cases

This repository contains real-world SIEM detection scenarios, complete with sample logs, detection logic, and response recommendations. It’s designed for SOC analysts, blue teamers, and cybersecurity learners who want to understand how common threats appear in logs and how to detect them using a SIEM platform.

---

## 🧠 What is a SIEM?

A **Security Information and Event Management (SIEM)** system collects, normalizes, and analyzes log data from across an organization’s IT environment. SIEM platforms help detect threats, investigate incidents, and support compliance efforts by providing real-time alerts, dashboards, and centralized visibility into security-relevant events.

In practice, a SIEM ingests logs from sources like:

- Windows Event Logs and Sysmon
- Firewalls, routers, and IDS/IPS devices
- Cloud services and authentication systems (e.g., Azure AD, Okta)
- Applications and databases

By correlating data from different systems, SIEMs enable security teams to identify suspicious behavior that might otherwise go unnoticed.

---

## 🛠️ Common SIEM Platforms

- **Splunk** – A powerful, enterprise-grade SIEM known for its scalability, flexible query language (SPL), and app ecosystem.
- **Microsoft Sentinel** – A cloud-native SIEM in Azure that integrates seamlessly with Microsoft 365, Defender, and Azure resources.
- **Elastic Security (ELK Stack)** – Open-source stack (Elasticsearch, Logstash, Kibana) used for log analysis and detection engineering.
- **IBM QRadar** – Popular in large enterprises for correlation rules and built-in threat intelligence.
- **LogRhythm** – Known for its ease of use and unified monitoring capabilities.

Whether you're defending an enterprise network or building a lab, understanding how SIEMs interpret and detect common attack patterns is a critical skill for modern cybersecurity professionals.

---

## 🔍 What's Included

Each folder covers a different detection use case and typically includes:

- 📁 Sample logs (Windows Event Logs, Sysmon, firewall, etc.)
- 🔍 Detection logic (Sigma rules, queries, or pseudocode)
- 🧠 Explanation of what the event means
- 🔐 MITRE ATT&CK technique mapping
- 🛠️ Recommended triage and response steps

---

## 📁 Example Use Cases

| Detection Scenario                     | Description                                           | Platforms/Log Types       |
|----------------------------------------|-------------------------------------------------------|---------------------------|
| 🔐 Failed Windows Login Attempts        | Detect repeated login failures                        | Windows / Active Directory |
| 🛠️ PowerShell Obfuscation Detection     | Look for encoded or suspicious PowerShell commands    | Sysmon                    |
| 🚨 Brute Force Authentication Attempts  | High volume of failed logins by a single user/IP      | Windows/Linux             |
| 🔗 Lateral Movement via PSExec/SMB      | Monitor use of remote execution tools                 | Sysmon / Windows Security |
| 🌐 Suspicious DNS Queries               | Query patterns matching C2 activity                   | DNS Logs                  |
| 📤 Data Exfiltration via FTP/HTTP       | Large outbound transfers or uploads                   | Proxy / Firewall          |
| 📁 USB Drive Activity Detection         | Alert on external storage insertion or file transfer  | Windows Event Logs        |

---

## 🎯 Goals

- Help blue teams understand how attacks show up in logs
- Provide a starting point for building detections in SIEM platforms
- Encourage mapping detections to MITRE ATT&CK
- Assist in creating practical blue team labs and training

---

## 🚀 How to Use

1. Choose a folder for a specific use case.
2. Review the sample logs and read the detection explanation.
3. Modify the detection logic for your SIEM (Splunk, Sentinel, ELK, etc.).
4. Test and adapt to your environment.
5. Apply triage steps and consider automation where appropriate.

---

## 🔗 Related Projects

- [Cybersecurity HTTP Status Code Guide](https://github.com/cherinejoseph/http-status-codes-for-cybersecurity-it)
- [OWASP Top 10 Security Risks Guide](https://github.com/your-username/OWASP-Top-10-Security-Risks)

---

## 🙋‍♀️ Contribute

Have a log source or detection you'd like to share?  
Feel free to fork the repo, add your scenario folder, and submit a pull request.
