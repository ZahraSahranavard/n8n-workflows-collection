# 📌 Google Sheet Field Transformation 

This workflow demonstrates data transformation and field manipulation using Google Sheets inside n8n.

It retrieves rows from a spreadsheet and dynamically modifies fields using expressions and JavaScript logic.



## ⚡ What This Workflow Does

1. Fetches rows from Google Sheets
2. Creates a new `Fullname` field
3. Converts last name to uppercase
4. Increases age by 10
5. Outputs structured and transformed data

This project highlights real-time data transformation capabilities in n8n.



## 🛠 Technologies

- n8n – Workflow Automation
- Google Sheets API
- Built-in n8n Nodes:
  - Manual Trigger
  - Google Sheets
  - Set (Field Transformation)



## 🧠 Workflow Logic

### 1️⃣ Manual Trigger
Starts the workflow manually.

### 2️⃣ Get row(s) in sheet
Retrieves records from Google Sheets.

Example input fields:
- Firstname
- Lastname
- Age
- Gender

### 3️⃣ Edit Fields (Set Node)

Transforms data using expressions:

- `Fullname`
- `Age`
- `gender`  


This demonstrates:
- String manipulation
- JavaScript expressions
- Numeric operations
- Field restructuring

## 🚀 How to Run

1. Import the JSON workflow into n8n  
 → Workflows → Import  

2. Create Google Sheets OAuth2 credential  

3. Replace:

4. Execute the workflow



## 🔐 Security

- This repository contains a sanitized version
- No real credentials included
- No real spreadsheet IDs included
- No sample personal data stored



## 📁 Node Structure

| Node | Purpose |
|------|----------|
| Manual Trigger | Start workflow |
| Google Sheets | Retrieve data |
| Set (Edit Fields) | Transform and manipulate fields |