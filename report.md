SOC Incident Report – Phishing Campaign Analysis
📌 Incident Summary

A multi-stage phishing campaign targeting Spanish banking users (KutxaBank) was identified.

The campaign leveraged:

compromised infrastructure
cloaking techniques
credential harvesting mechanisms

🎯 Objective
Harvest banking credentials (NIF/NIE and password)
Potentially capture OTP for account takeover

🔗 Attack Chain
Phishing email sent from a compromised account
Redirect through a compromised legitimate website
Conditional cloaking and anti-analysis behavior
Fake CAPTCHA page used as a filtering mechanism
Final phishing login page (credential harvesting)

🧩 Indicators of Compromise (IoCs)

📧 Email
antrian-rsub@ub.ac.id

🌐 Domains
chantaygiavietnam.com
ch239305.tw1.ru

🌍 IP
103.7.40.181

⚙️ Techniques Observed
Abuse of legitimate email infrastructure (SPF, DKIM, DMARC valid)
Cloaking / conditional redirection
Multi-stage redirection chain
Fake CAPTCHA (anti-analysis technique)
Credential harvesting via phishing page

🧠 Threat Actor Assessment
Skill Level: Intermediate
Capabilities:
Infrastructure chaining
Evasion techniques
Credential harvesting

🚨 Impact
High risk of credential theft
Potential financial fraud
Increased effectiveness due to trusted domains
🛠️ Recommendations
For Organizations
Enforce Multi-Factor Authentication (MFA)
Monitor unusual login activity
Audit outbound email traffic
For Website Owners
Scan for malicious scripts
Review server logs
Update CMS and plugins
Reset credentials

📊 MITRE ATT&CK Mapping
T1566.002 – Phishing (Link)
T1078 – Valid Accounts
T1189 – Drive-by Compromise
T1204 – User Execution

🧾 Conclusion

This phishing campaign demonstrates the use of compromised infrastructure and evasion techniques to bypass detection and increase success rates.

It represents a real-world example of modern phishing operations.
