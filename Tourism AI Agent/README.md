# 📌 Tourism AI Agent

This n8n workflow is a **Tourism Assistant** bot that uses **AI Agent + Memory + Tools** to answer questions related to travel, cities, and tourism activities. It demonstrates **Automation + AI Integration** and can be used as a portfolio project.



## ⚡ Features

- Receives chat messages using **Chat Trigger** node  
- Processes messages via **AI Agent** connected to **Google Gemini (PaLM)**  
- Uses **Memory Buffer** to keep the context of the last 10 messages  
- Can call **Wikipedia** for historical queries  
- Can perform calculations using **Calculator** tool  
- Extensible workflow for adding more tools and capabilities  



## 🛠 Technologies

- [n8n](https://n8n.io/) – Workflow Automation  
- [Google Gemini (PaLM)](https://developers.generativeai.google/) – LLM Integration  
- LangChain Nodes for AI Agent, Memory, and Tools  


## 🚀 How to Run

1. **Import the JSON file in n8n:**  
   - Go to **Workflows → Import**  
   - Select the JSON file


2. **Set up Credentials in n8n:**  
   - Google Gemini API → enter your API key  


3. **Activate the Workflow:**  
   - Turn on the workflow and start chatting with the bot  



## 🔐 Security

- This is a **safe GitHub template**  
- No real API keys, webhook IDs, or credentials are included  
- You must add your own credentials before running  



## 📁 Node Structure

| Node Name                     | Purpose |
|--------------------------------|---------|
| When chat message received     | Receive user messages |
| AI Agent                       | Process messages and generate responses |
| Google Gemini Chat Model       | LLM processing |
| Simple Memory                  | Maintain context of last messages |
| Wikipedia                      | Provide historical information |
| Calculator                     | Perform mathematical calculations |

