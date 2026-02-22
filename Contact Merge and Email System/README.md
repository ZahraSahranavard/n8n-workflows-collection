# 📌 Contact Merge and Email System

This workflow demonstrates  data processing in n8n using:

- Multiple Google Sheets sources
- Data transformation
- Merge operations
- Field splitting
- Automated email sending via Gmail

It showcases real-world automation logic for CRM, marketing, and customer communication systems.



## ⚡ What This Workflow Does

1. Fetches data from **two separate Google Sheets**
2. Standardizes fields from different schemas
3. Merges both datasets into one unified stream
4. Splits output per email address
5. Sends automated emails to each recipient

This is a practical example of multi-source data normalization and automation.



## 🛠 Technologies

- n8n – Workflow Automation
- Google Sheets API
- Gmail API
- Built-in n8n Nodes:
  - Manual Trigger
  - Google Sheets
  - Set (Data Transformation)
  - Merge
  - Split Out
  - Gmail



## 🧠 Workflow Architecture

### 1️⃣ Manual Trigger
Starts the workflow manually.

### 2️⃣ Get Sheet 1
Retrieves dataset #1:
- firstname
- lastname
- email

### 3️⃣ Get Sheet 2
Retrieves dataset #2:
- Name
- Family
- Contact

### 4️⃣ Data Normalization (Set Nodes)
Both datasets are transformed into a unified structure:

- `Fullname`
- `Email`

This step ensures compatibility before merging.

### 5️⃣ Merge Node
Combines both processed datasets into a single stream.

### 6️⃣ Split Out Node
Splits the dataset per `Email`, preparing individual email sends.

### 7️⃣ Gmail Node
Sends an automated message to each email address.



## 🚀 How to Run

1. Import the JSON workflow file into n8n  
   → Workflows → Import  


2. Create Credentials:
   - Google Sheets OAuth2
   - Gmail OAuth2  


3. Replace:
    - YOUR_GOOGLE_SHEET_ID


4. Customize email:
   - Subject
   - Message body


5. Click **Execute Workflow**



## 🔐 Security

- This repository contains a sanitized version.
- No credentials are included.
- No real spreadsheet IDs are included.
- No personal email data is stored.
- Users must configure their own OAuth credentials.



## 📁 Node Structure

| Node | Purpose |
|------|----------|
| Manual Trigger | Start workflow |
| Google Sheets (x2) | Fetch data from two sources |
| Set (x2) | Normalize data structure |
| Merge | Combine datasets |
| Split Out | Split per email |
| Gmail | Send email |


## 🌟 Real-World Use Cases

- CRM email campaigns
- Multi-database contact synchronization
- Newsletter automation
- Marketing outreach
- Internal communication automation




