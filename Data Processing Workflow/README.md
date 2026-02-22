# 📌 Data Processing Workflow

This n8n workflow demonstrates basic but powerful data processing operations using **Google Sheets + Sort + Wait + Limit** nodes.

It is designed as a simple example of data automation and transformation inside n8n and can be used as a portfolio project.



## ⚡ Features

- Manually triggered workflow  
- Fetch data from Google Sheets  
- Sort rows by a specific field (Age)  
- Wait for a defined time (10 seconds)  
- Limit output to a specific number of items (Top 5)  



## 🛠 Technologies

- [n8n](https://n8n.io/) – Workflow Automation  
- Google Sheets API  
- Built-in n8n Nodes:
  - Google Sheets
  - Sort
  - Wait
  - Limit



## 🚀 How to Run

1. **Import the JSON file into n8n**
   - Go to **Workflows → Import**
   - Select the workflow JSON file

2. **Set up Google Sheets Credentials**
   - Create a Google Sheets OAuth2 credential
   - Connect your Google account

3. **Add Your Google Sheet ID**
   - In the `Get row(s) in sheet` node
   - Replace `YOUR_GOOGLE_SHEET_ID` with your actual Sheet ID

4. **Execute the Workflow**
   - Click **Execute workflow**
   - The workflow will:
     - Fetch rows
     - Sort them by Age
     - Wait 10 seconds
     - Return the first 5 items



## 🔐 Security

- This is a **sanitized GitHub template**
- No real credentials or sheet IDs are included
- You must add your own Google credentials before running



## 📁 Node Structure

| Node Name | Purpose |
|-----------|----------|
| Manual Trigger | Start workflow manually |
| Google Sheets | Retrieve rows from spreadsheet |
| Sort | Sort data by Age |
| Wait | Pause execution for 10 seconds |
| Limit | Return only first 5 items |

