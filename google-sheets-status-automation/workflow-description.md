# 🔄 Google Sheets Advanced Automation (Zapier Workflow)

This Zapier workflow automates data processing in Google Sheets using multiple steps including data fetching, JavaScript logic, filtering, and updating rows automatically.

---

## 🚀 Workflow Overview

This automation triggers when a Google Sheets row is **created or updated**, processes multiple rows, applies custom JavaScript logic, filters conditions, and finally updates the spreadsheet accordingly.

---

## ⚙️ Workflow Steps

### 1️⃣ Trigger: New or Updated Spreadsheet Row
- App: Google Sheets  
- Event: New or Updated Spreadsheet Row  
- This step triggers the automation whenever a row is added or modified.

---

### 2️⃣ Action: Get Many Spreadsheet Rows
- App: Google Sheets  
- Event: Get Many Spreadsheet Rows  
- Fetches multiple rows from the sheet for comparison or batch processing.

---

### 3️⃣ Code Step: Run JavaScript (Code by Zapier)
- App: Code by Zapier  
- Event: Run JavaScript  
- Performs custom logic such as:
  - Data comparison  
  - Condition checking  
  - Status validation  
  - Row processing logic  

---

### 4️⃣ Filter Step: Filter Conditions
- App: Filter by Zapier  
- Only allows data to continue if specific conditions are met  
- Example conditions:
  - All items are posted  
  - Status matches required value  
  - Data is complete  

---
## 🧠 Business Logic (Important Condition)

This workflow is designed with a strict condition check:

### ✅ Rule:
The system will ONLY update all rows to **"Pending"** when:

- ✔️ ALL rows have status = **"Posted"**

---

### ❌ It will NOT run if:

- ❌ Even **1 row is "Pending"**
- ❌ OR all rows are already "Pending"
- ❌ OR mixed status exists (Posted + Pending)

---

### ⚙️ Logic Explanation:

The JavaScript step checks the entire dataset from Google Sheets.

It verifies:

- Are ALL rows marked as "Posted"?

👉 If YES → then update ALL rows to **"Pending"**

👉 If NO → do NOTHING (no update happens)

---

### 🎯 Purpose of This Logic:

- Prevents accidental updates  
- Ensures full completion before status reset  
- Maintains data accuracy  
- Avoids partial or mixed-state processing  

---

### 5️⃣ Action: Update Spreadsheet Row(s)
- App: Google Sheets  
- Event: Update Spreadsheet Row(s)  
- Updates the final status or processed result back into the sheet  
- Example: changing status to **"Posted"**, **"Completed"**, or **"Processed"**

---

## 🎯 Purpose of This Automation

- Automates Google Sheets data validation  
- Reduces manual tracking work  
- Ensures accurate status updates  
- Applies custom logic using JavaScript  
- Improves workflow efficiency for bulk data

---

## 🧠 Key Features

- Multi-row processing  
- Custom JavaScript logic support  
- Conditional filtering system  
- Automatic status updates  
- Fully no-code + low-code hybrid automation  

---

## 📌 Use Cases

- Social media post tracking system  
- Task completion monitoring  
- Inventory or data status updates  
- Workflow automation dashboards  
- Batch data processing in Google Sheets  

---

## ⚡ Result

Once all conditions are satisfied, the workflow automatically updates the relevant Google Sheets rows without manual intervention.

---
