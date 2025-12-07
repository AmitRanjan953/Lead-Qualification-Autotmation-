# 🚀 AI-Powered Lead Qualification Automation (n8n Workflow)

This project is an **end-to-end AI-powered Lead Qualification Automation system built using n8n**.  
It automatically captures leads from Google Forms, classifies them using **Google Gemini AI**, stores them in Google Sheets, sends confirmation emails, and instantly alerts you on Telegram for **Hot Leads**.

---

## ✅ Features

- 📥 **Automatic Lead Capture** from Google Sheets (Google Form responses)
- 🤖 **AI-Based Lead Scoring** using Google Gemini API
- 🔥 **Lead Classification** into:
  - Hot
  - Warm
  - Cold
- 📊 **Auto Storage in Google Sheets CRM**
- 📩 **Automated Thank You Email** using Gmail
- 📲 **Instant Telegram Alerts for Hot Leads**
- 🕒 **Automatic Timestamp Logging**
- ✅ **Fully No-Code + AI Integrated System**

---

## 🧩 Workflow Architecture

Google Form → Google Sheets Trigger →  
JavaScript Processing → Gemini AI Classification →  
✅ Store in CRM Sheet  
✅ Email to Lead  
✅ Telegram Alert (Only for HOT leads)

---

## 🛠️ Tech Stack Used

- **Automation Tool:** n8n  
- **AI Model:** Google Gemini (PaLM API)  
- **Database:** Google Sheets  
- **Notification:** Telegram Bot  
- **Email Service:** Gmail  
- **Logic Processing:** JavaScript (n8n Code Node)

---

## 📂 Workflow Nodes Explained

| Node | Purpose |
|------|---------|
| Google Sheets Trigger | Detects new lead from form |
| JavaScript Code Node | Cleans and structures lead data |
| HTTP Request | Sends data to Gemini AI for scoring |
| IF Node | Filters HOT leads |
| Google Sheets Append | Saves lead to CRM |
| Gmail Node | Sends confirmation email |
| Telegram Node | Sends HOT lead alert |

---

## 📥 Input Lead Fields

- Name
- Email
- Phone
- Company

---

## 📤 Output Fields Stored

- Name
- Email
- Phone
- Company
- Lead Score (Hot/Warm/Cold)
- AI Notes
- Timestamp

---

## 🔔 Telegram Alert Example

🔥 New HOT Lead Alert!  
Name: John Doe  
Email: john@email.com  
Phone: 9876543210  
Company: ABC Pvt Ltd  
Score: Hot  
Reason: Strong business intent detected  

---

## 📧 Auto Email Sent to Lead

Subject: Thank You!  
Message:
Hi {{Name}},  
Thank you for reaching out! Our team will get in touch with you shortly.  
Regards, Amit

---

## ⚙️ Setup Instructions

1. Import the JSON workflow into your n8n instance  
2. Connect credentials:
   - Google Sheets
   - Gmail
   - Telegram Bot
   - Google Gemini API
3. Update:
   - Telegram Chat ID
   - Google Sheet IDs
4. Activate the workflow ✅

---

## 🔒 Security Notes

- Never expose your API keys in public repos
- Use environment variables for production
- Restrict Telegram bot access

---

## 🎯 Use Cases

- SaaS Lead Management
- Sales CRM Automation
- Real Estate Leads
- Digital Marketing Agencies
- Startup Lead Tracking

---

## 👨‍💻 Author

**Amit Ranjan Gupt**  
B.Tech (CSE - AI & ML)  


---

## ⭐ If you like this project, give it a star!


