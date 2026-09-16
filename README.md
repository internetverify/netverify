# NetVerify — Community Threat Intelligence & Takedown Feed

NetVerify is a 100% independent, non-profit internet safety initiative dedicated to identifying, investigating, and mitigating malicious online infrastructure. 

Our core mission is to actively take down fraudulent websites, banking scams, and phishing campaigns to keep everyday internet users safe — entirely free of charge.

🌐 **Official Portal:** https://netverify.org.in

---

## 🛡️ What This Repository Contains

This repository serves as our public transparency ledger and threat intelligence distribution point:
- **Verified Takedown Ledger:** We publish verified telemetry of malicious sites that we have either taken down directly or successfully coordinated with hosting providers and domain registrars to mitigate.
- **Monthly Feed Updates:** Our incident telemetry is compiled and updated monthly inside `data/feed.csv` for security researchers, DNS resolvers, and network administrators.
- **Takedown Telemetry:** Each entry reflects real-time status actions such as `clientHold`, `serverHold`, and `hosting_suspended`.

---

## ⚡ Incident Response & SLA

We take every incident seriously and operate with rapid triage protocols:
- **48-Hour SLA Guarantee:** Every scam/phishing report submitted to our triage desk receives an initial review and response within **48 hours**.
- **Evidence Verification:** Our automated and manual verification layers inspect DNS routing, host infrastructure, and active malicious payloads before dispatching abuse alerts to upstream authorities.

> *Note: The NetVerify front-end ingestion engine and internal triage scripts remain private to prevent threat actors from spoofing or cloning our brand. This repository maintains our open public threat data and community parsers.*

---

## 📊 Telemetry Feed Schema (`data/feed.csv`)

| Column | Description |
| :--- | :--- |
| `domain` | Fully Qualified Domain Name (FQDN) of the malicious target |
| `type` | Classification (e.g., `phishing`, `banking_scam`, `malware`) |
| `threat_level` | Severity assessment (`low`, `medium`, `high`, `critical`) |
| `action_taken` | Mitigation status (`suspended`, `clientHold`, `serverHold`) |
| `reported_date` | Date of logged mitigation action (YYYY-MM-DD) |

---

## 📬 Contact & Reporting Channels

- **Submit Abuse / Phishing Reports:** [report@p.netverify.org.in](mailto:report@p.netverify.org.in)
- **General Support & Inquiries:** [support@netverify.org.in](mailto:support@netverify.org.in)
- **Official Inquiries & Partnerships:** [official@netverify.org.in](mailto:official@netverify.org.in)

---

## 📄 License
This threat feed is open data published under the [MIT License](LICENSE). Free for researchers, enterprise blocklists, and community defenders.
