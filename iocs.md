# Indicators of Compromise (IoCs)

---

## 📧 Email Indicators
- antrian-rsub@ub.ac.id

---

## 🌐 Domain Indicators
- chantaygiavietnam.com
- ch239305.tw1.ru

---

## 🌍 IP Indicators
- 103.7.40.181

---

## ⚙️ Observed Techniques
- Cloaking (environment-based filtering)
- Fake CAPTCHA (anti-analysis)
- Multi-stage redirection
- Credential harvesting (bank impersonation)

---

## 🧠 Context

These IoCs are associated with a phishing campaign targeting banking users.

The attack chain includes:
- compromised infrastructure
- redirection mechanisms
- credential harvesting techniques

---

## 🛡️ Detection Notes
- Monitor outbound emails from trusted domains
- Flag connections to newly observed domains
- Detect suspicious redirection chains
- Identify login forms hosted outside legitimate domains
