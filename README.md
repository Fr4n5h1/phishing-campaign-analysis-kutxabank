Phishing Campaign Analysis – KutxaBank

Real-world phishing campaign analysis with cloaking, multi-stage redirection and credential harvesting (SOC-style report)

🚨 Key Findings
Compromised email account used for phishing distribution
Multi-stage redirection via compromised website
Cloaking techniques to evade sandbox detection
Fake CAPTCHA used as anti-analysis mechanism
Credential harvesting targeting banking users

📌 Overview

This repository documents the analysis of a real-world phishing campaign targeting Spanish banking users.

The campaign leveraged:

compromised infrastructure
cloaking techniques
multi-stage redirection
credential harvesting

🎯 Objectives of the Analysis
Identify the attack chain
Extract indicators of compromise (IoCs)
Understand evasion techniques used by the attacker
Document findings in a structured SOC-style report

🔗 Attack Chain

Email → Compromised Domain → Cloaking → Fake CAPTCHA → Phishing Login

Phishing email sent from a compromised domain
Redirect through a legitimate but compromised website
Conditional cloaking and anti-analysis behavior
Fake CAPTCHA page to filter victims
Final credential harvesting page (bank login clone)
📸 Evidence
Phishing Email




Fake CAPTCHA




Phishing Login Page




🧠 Techniques Observed
Abuse of legitimate email infrastructure (SPF/DKIM/DMARC valid)
Multi-stage redirection
Cloaking / sandbox evasion
Fake CAPTCHA as anti-analysis gate
Credential harvesting (bank impersonation)

🛡️ Detection Opportunities
Monitor unusual outbound emails from trusted domains
Detect redirections to newly observed domains
Identify fake CAPTCHA patterns
Flag login pages served from non-legitimate domains

🧩 Indicators of Compromise (IoCs)

📧 Email
antrian-rsub@ub.ac.id

🌐 Domains
chantaygiavietnam.com
ch239305.tw1.ru

🌍 IP
103.7.40.181

🛠️ Tools Used
VirusTotal
URLScan
ANY.RUN
Manual header analysis

💡 Why this matters

This campaign demonstrates how attackers:

abuse legitimate infrastructure
bypass detection systems
increase success rate through trust exploitation

⚠️ Disclaimer

This analysis is for educational and defensive purposes only.
No interaction with malicious infrastructure was performed beyond controlled analysis environments.

📄 Full Report

See report.md
