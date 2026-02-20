# 📌 Medical Assistant Telegram Bot

**Medical Assistant** is a Telegram bot that uses **n8n** and **LLM (Large Language Model)** to answer general medical questions. This project demonstrates **Automation + AI Agent Integration** and can be used as a portfolio piece on your resume.

---

## ⚡ Features

- Connects to **Telegram** to receive messages  
- Processes messages with **LLM (OpenRouter / GPT-3.5-turbo)**  
- Smart system for answering general medical questions  
- **Memory Buffer** keeps the context of recent messages  
- Extensible workflow for adding more Nodes and features  

---

## 🛠 Technologies

- [n8n](https://n8n.io/) – Workflow Automation  
- [OpenRouter](https://openrouter.ai/) – LLM Integration  
- Telegram Bot API  
- LangChain Node in n8n for AI model management  

---

## 🚀 How to Run

1. **Clone the repository:**

```bash
git clone https://github.com/YOUR_USERNAME/AIAgent_n8n_template.git
cd AIAgent_n8n_template
```

2. **Import the JSON file in n8n:**  
   - Go to **Workflows → Import**  
   - Select the JSON file


3. **Set up Credentials in n8n:**  
   - Telegram API → enter your bot token  
   - OpenRouter API → enter your API key


4. **Set Telegram chatId:**  
   - In the `Send a text message` Node, replace `YOUR_TELEGRAM_CHAT_ID` with the real chat ID  


5. **Activate the Workflow:**  
   - Turn on the workflow, and the bot is ready to respond to messages  

---

## 🔐 Security

- This is a **safe GitHub template**  
- No real API keys, webhook IDs, or credentials are included  
- You must add your own credentials before running  

---

## 📁 Node Structure

| Node Name                | Purpose |
|---------------------------|---------|
| Telegram Trigger          | Receive messages from users |
| AI Agent                  | Process messages and decide response |
| OpenRouter Chat Model     | Run the LLM |
| Simple Memory             | Keep context of recent messages |
| Send a text message       | Send reply to user |