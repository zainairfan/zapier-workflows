AI Email Classifier & Automated Alert System
---

This project is an intelligent automation workflow built on Zapier that uses AI to classify incoming emails and manage them based on their category (e.g., Information, Spam, Urgent). It ensures that important data is logged and critical alerts are sent out instantly.

---
🔄 Workflow Logic
--
As shown in the technical flow in image_89b4d5.png, the system operates as follows:

-New Email (Gmail): Monitors the inbox for any new incoming mail.

-AI Classification (AI by Zapier): The AI analyzes the email body to determine its nature. It classifies the email into categories such as:

- Inquiry/Info

- Spam

- Action Required

-Data Logging (Google Sheets): Every classified email is recorded in a Google Sheet, capturing the sender's details, the AI-generated category, and a summary.

-Filter (Filter by Zapier): The system checks the AI's classification. It is configured to only allow high-priority or relevant categories to pass through to the next step.

-Instant Alert (Gmail): If the email is classified as important, an automated alert email is sent to the relevant team or person to ensure a quick response.

---

✨ Key Features
---
Intelligent Categorization: Uses AI to distinguish between "Info" and "Spam" without manual effort.

Centralized Database: Automatically builds a history of all communications in Google Sheets.

Priority Filtering: Ensures you only get notified about emails that actually matter.

Real-time Alerts: Reduces response time by sending instant notifications for critical emails.

---
🛠️ Tech Stack
--
Zapier: Workflow Automation.

AI by Zapier: Natural Language Processing (NLP) for classification.

Gmail: Email Trigger and Alert System.

Google Sheets: Database and Logging.
