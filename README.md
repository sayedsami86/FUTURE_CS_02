# FUTURE_CS_02 — Phishing Email Detection & Awareness Report
## Future Interns | Cyber Security Track | Task 2

![Cyber Security](https://img.shields.io/badge/Cyber%20Security-Internship-blue)
![Phishing](https://img.shields.io/badge/Domain-Phishing%20Detection-red)
![Status](https://img.shields.io/badge/Status-Completed-green)

---

## 📋 Task Overview

**Task:** Phishing Email Detection & Awareness System  
**Emails Analyzed:** 6 samples (5 phishing/suspicious, 1 legitimate)  
**Tools Used:** MXToolbox Header Analyzer, Browser DevTools, Manual Analysis  
**Assessment Date:** May 2, 2026  
**Intern:** Mohammad Sami Sadiq Ali Sayed  

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| MXToolbox Header Analyzer | Email header analysis (SPF, DKIM, DMARC) |
| Browser DevTools | Link inspection & URL analysis |
| Manual Analysis | Phishing indicator identification |

---

## 📧 Email Classification Results

| # | Subject | From | Classification | Risk |
|---|---------|------|---------------|------|
| 1 | URGENT: Your SBI account has been suspended | security@sbi-alert-verify.com | 🔴 PHISHING | CRITICAL |
| 2 | You have been selected for Infosys | hr@infosys-careers-india.net | 🔴 PHISHING | HIGH |
| 3 | Your Microsoft account will be deleted | no-reply@microsoft-security-center.com | 🔴 PHISHING | HIGH |
| 4 | You won ₹50,000! Claim your prize | winner@amazon-lucky-draw-india.com | 🔴 PHISHING | CRITICAL |
| 5 | Induction Session Details Innovexis Internship | juv.innovexis.in | 🟠 SUSPICIOUS | MEDIUM |
| 6 | Your GitHub repository has a new commit | no-reply@github.com | 🟢 SAFE | NONE |

---

## 🔍 Key Phishing Indicators Found

### Red Flags Identified Across Samples:
- ❌ **Spoofed domains** — fake domains mimicking SBI, Infosys, Microsoft, Amazon
- ❌ **Urgency tactics** — "URGENT", "suspended", "deleted in 24 hours"
- ❌ **Suspicious TLDs** — .xyz, .tk, .net used instead of official .com/.in
- ❌ **Payment requests** — asking for ₹500 "registration fee" for fake job offer
- ❌ **Bank detail requests** — requesting account numbers for fake prize
- ❌ **Typosquatting** — "microsft-login.com" (missing 'o' in Microsoft)
- ⚠️ **DMARC failure** — real email header showed DMARC fail despite SPF/DKIM pass

---

## 📊 Real Header Analysis — Email 5

**Tool Used:** MXToolbox Email Header Analyzer  
**Subject:** Induction Session Details Innovexis Internship  

| Check | Result |
|-------|--------|
| DMARC | ❌ FAILED |
| SPF Alignment | ✅ Pass |
| SPF Authenticated | ✅ Pass |
| DKIM Alignment | ✅ Pass |
| DKIM Authenticated | ✅ Pass |
| Relay | juv.innovexis.in → mx.google.com |

**Classification: SUSPICIOUS** — DMARC failure despite SPF/DKIM pass indicates domain misconfiguration or possible spoofing.

---

## 🛡️ Key Prevention Guidelines

1. **Verify sender domain** — not just the display name
2. **Hover before clicking** — preview URLs before visiting
3. **Never pay for job offers** — legitimate companies never ask for fees
4. **Check for typosquatting** — look for misspellings in URLs
5. **Enable MFA** — on all important accounts
6. **Report phishing** — cybercrime.gov.in (India)

---

## 📁 Repository Contents

```
FUTURE_CS_02/
├── README.md                              # This file
├── FUTURE_CS_02_Phishing_Report.docx      # Full phishing detection report
└── screenshots/
    └── mxtoolbox_header_analysis.png      # Real email header analysis result
```

---

## 👤 About the Intern

**Mohammad Sami Sadiq Ali Sayed**  
BSc IT Graduate | CGPA: 8.43 | Aspiring Penetration Tester  
📧 sayedsami86@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/mohammed-sami-sayed-b702673b7)  

---

*This assessment was performed for educational purposes as part of the Future Interns Cyber Security Internship Program.*
