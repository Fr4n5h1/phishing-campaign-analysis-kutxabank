# phishing-campaign-analysis-kutxabank
Real-world phishing campaign analysis with cloaking, multi-stage redirection and credential harvesting (SOC-style report)

📌 Overview

This repository documents the analysis of a real-world phishing campaign targeting Spanish banking users.
The campaign leveraged compromised infrastructure, cloaking techniques, and multi-stage redirection to harvest credentials.

🎯 Objectives of the Analysis
Identify the attack chain
Extract indicators of compromise (IoCs)
Understand evasion techniques used by the attacker
Document findings in a structured SOC-style report
🔗 Attack Chain
Phishing email sent from a compromised domain
Redirect through a legitimate but compromised website
Conditional cloaking and anti-analysis behavior
Fake CAPTCHA page to filter victims
Final credential harvesting page (bank login clone)
🧠 Techniques Observed
Abuse of legitimate email infrastructure (SPF/DKIM/DMARC valid)
Multi-stage redirection
Cloaking / sandbox evasion
Fake CAPTCHA as anti-analysis gate
Credential harvesting (bank impersonation)
🧩 Indicators of Compromise (IoCs)
Type	Value
Email	antrian-rsub@ub.ac.id
Domain	chantaygiavietnam.com
IP	103.7.40.181
Phishing	ch239305.tw1.ru
🛠️ Tools Used
VirusTotal
URLScan
ANY.RUN
Manual header analysis
⚠️ Disclaimer

This analysis is for educational and defensive purposes only.
No interaction with malicious infrastructure was performed beyond controlled analysis environments.

📄 Full Report

See report.md
