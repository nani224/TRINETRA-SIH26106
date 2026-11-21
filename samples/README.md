# 🧪 TRINETRA Calibrated Test Email & Message Samples

This directory provides a suite of pre-calibrated test cases across RFC 822 `.eml` and Outlook binary / MIME `.msg` formats. These files are specifically engineered to demonstrate and test TRINETRA's **3-Layer Risk Fusion Engine**, multi-script Indic NLP, header forensics, and legal dossier generation.

---

## 📊 Summary of Test Cases & Calibrated Risk Scores

| File Name | Format | Target Threat Category | Calibrated Score | Triggered Security Indicators |
| :--- | :---: | :--- | :---: | :--- |
| `01_score_20_clean_college_announcement.eml` | `.eml` | **Clean / Legitimate** | **20 / 100** | Strict SPF/DKIM/DMARC pass, legitimate institutional domain (`vce.ac.in`), zero urgency, normal internal IP hops. |
| `02_score_20_clean_project_meeting.msg` | `.msg` | **Clean / Legitimate** | **20 / 100** | Departmental review schedule, verified relay headers, clean body semantics, no suspicious URLs or attachments. |
| `03_score_50_moderate_vendor_invoice.eml` | `.eml` | **Moderate / Suspicious** | **~50 / 100** | Financial context, soft DMARC neutral/none, invoice update urgency, external routing. |
| `04_score_50_moderate_hr_benefits_review.msg` | `.msg` | **Moderate / Suspicious** | **~50 / 100** | Internal HR policy update link, moderate corporate urgency, generic sender mismatch. |
| `05_score_70_high_sbi_bank_kyc_phishing.eml` | `.eml` | **High Threat** | **~75 / 100** | Banking KYC suspension threat, typosquatted banking domain, urgent account freeze call to action, relay spoofing. |
| `06_score_70_high_o365_credential_harvesting.msg` | `.msg` | **High Threat** | **~73 / 100** | Fake Microsoft 365 password expiry notice, external credential harvesting link, SPF failure. |
| `07_score_100_critical_digital_arrest_extortion.eml` | `.eml` | **Critical Threat** | **100 / 100** | Fake CBI / Cyber Crime arrest warrant, coercive Hindi/English extortion text, forged government headers, Tor/VPN relay hop. |
| `08_score_100_critical_executive_wire_fraud.msg` | `.msg` | **Critical Threat** | **99–100 / 100** | CEO/Executive impersonation, urgent secret acquisition wire transfer request, complete SPF/DKIM failure, spoofed display name. |

---

## 🚀 How to Test in the Live Dashboard

1. Open the TRINETRA SOC Analyst Dashboard at **`http://localhost:5173`**.
2. Drag and drop any of the files from this directory into the **Email Upload** zone (or use the one-click presets).
3. Observe:
   - **Score Gauge**: Immediate threat score matching the calibrated risk tier.
   - **Hop-0 Geolocation**: Origin tracing displaying the sender host IP and geo-coordinates on Leaflet.
   - **Protocol Diagnostics**: SPF, DKIM, and DMARC verification pills.
   - **Indic NLP Reasoning**: Threat vector breakdown (Urgency, Coercion, Financial, Impersonation).
   - **Court Dossier Export**: Click **Export Section 63 BSA Dossier** to generate a court-admissible forensic certificate with SHA-256 seal.
