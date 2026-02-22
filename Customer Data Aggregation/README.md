# 👥 Customer Data Aggregation

This n8n workflow demonstrates customer data processing using **Google Sheets + Data Transformation + Aggregation**.

It retrieves customer records from Google Sheets, formats selected fields, and aggregates structured output for reporting or automation use cases.



## ⚡ Features

- Manual workflow trigger
- Fetch customer records from Google Sheets
- Combine `firstname` and `lastname` into `Fullname`
- Extract key fields (Email, Country)
- Aggregate selected data fields
- Structured output ready for reporting or further automation



## 🛠 Technologies Used

- [n8n](https://n8n.io/) – Workflow Automation Platform
- Google Sheets API
- Built-in n8n Nodes:
  - Manual Trigger
  - Google Sheets
  - Set (Edit Fields)
  - Aggregate



## 🧠 Workflow Logic

1. **Manual Trigger**
   - Starts the workflow manually.

2. **Google Sheets – Get row**
   - Retrieves customer records from a spreadsheet.

3. **Edit Fields (Set Node)**
   - Creates:
     - `Fullname` = firstname + lastname
     - `Email`
     - `Country`

4. **Aggregate**
   - Outputs:
     - Customer's Name
     - Email
   - Data is structured for reporting or downstream workflows.



## 🚀 How to Run

1. Import the JSON file into n8n  
   → Workflows → Import  

2. Create Google Sheets Credentials  
   → Connect your Google account  

3. Replace:

YOUR_GOOGLE_SHEET_ID

with your actual Sheet ID.

4. Click **Execute workflow**



## 🔐 Security

- This is a sanitized GitHub template.
- No real credentials or spreadsheet IDs are included.
- No sample customer data is stored.
- You must configure your own credentials before running.


## 📁 Node Structure

| Node Name | Purpose |
|-----------|----------|
| Manual Trigger | Start workflow manually |
| Google Sheets | Retrieve customer rows |
| Edit Fields | Transform and structure data |
| Aggregate | Combine selected fields |