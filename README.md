# Elevate_Labs_Internship_Day_1-Task-2

# 📧 Phishing Email Analysis Report

This repository contains the analysis of a phishing email sample obtained from **Hook Security** for educational and awareness purposes.

> **Sample Source:** [Hook Security – Phishing Email Examples](https://www.hooksecurity.co/phishing-email-examples)  
> **Specific Example:** [Office 365 Phishing Example](https://www.hooksecurity.co/phishing-examples/office-365-phishing-example)  

⚠️ *Note: The sample is safe and intended for training — do not attempt to open links in real phishing emails.*

---

## 🔍 Step-by-Step Analysis

### **1. Examine the Sender’s Email Address**
- **Shown sender:** `UPS eNotification <amazon@update-nt.com>`  
- Domain `update-nt.com` is unrelated to UPS — strong sign of spoofing.  
- UPS official emails come from `@ups.com`.

---

### **2. Check Email Headers**
- Retrieve from email client (e.g., Gmail → “Show Original”).
- Use an [Email Header Analyzer](https://toolbox.googleapps.com/apps/messageheader/).
- Look for:
  - SPF/DKIM/DMARC failures.
  - “From” and “Return-Path” mismatches.
  - Suspicious IP addresses.

---

### **3. Identify Suspicious Links or Attachments**
- Tracking number hyperlink likely points to a malicious site.
- Hover over links without clicking to check the real destination.
- No attachments in this sample, but dangerous formats include `.exe`, `.zip`, `.docm`.

---

### **4. Look for Urgent or Threatening Language**
- Example: “If the package is not scheduled for delivery or picked up within 48 hours, it will be returned to the sender.”
- Creates pressure on the victim to act quickly.

---

### **5. Check for Mismatched URLs**
- Compare visible text to actual hyperlink URL.
- If different, this is a strong phishing sign.

---

### **6. Verify Spelling or Grammar Errors**
- Example: “Expected Deliver Date” (missing “y”).
- Awkward phrasing: “Printed shipping invoice mentioned below” (but no invoice attached).

---

## 📝 Summary Table of Phishing Traits

| Trait                  | Evidence |
|------------------------|----------|
| Fake sender domain     | `amazon@update-nt.com` instead of official UPS domain |
| Urgency tactic         | Threat of return in 48 hours |
| Suspicious link        | Tracking number hyperlink |
| Brand mismatch         | Mentions UPS but sender email says Amazon |
| Grammar errors         | “Expected Deliver Date” missing “y” |
| Missing personalization| “Dear,” without recipient name |

---


## 📜 License
This content is for **educational and awareness purposes only**.  
Do **not** reuse phishing emails in real-world campaigns.

