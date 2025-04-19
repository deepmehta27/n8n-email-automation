# n8n Automated Renewal Reminder
**Role:** AI Automation Intern • **Company:** ReAgent AI  

## 📋 Overview
This n8n workflow pulls pending contacts from **Google Sheets**, sends a personalised renewal‑reminder e‑mail via **Gmail**, and writes back `sent`/`error` status with timestamps (and Gmail `messageId` or `error_message`).

## 🚀 Quick Start
1. **Import** `email_automation_workflow.json` into your n8n instance  
2. **Create credentials**
   - *Google Sheets OAuth2* (readonly & write scopes)
   - *Gmail OAuth2* (send scope)
3. Copy the sample sheet template from `screenshots/CRM_template.png` *(or create your own)*  
4. **Run** the Manual Trigger – you’ll see rows change from `pending` → `sent`.

## 🗂️ CRM Used
- **Google Sheets** (one tab; headers: `first_name`, `email`, `company`, `last_product_purchased`, `renewal_date`, `email_status`, `last_contacted`, `error_message`).
