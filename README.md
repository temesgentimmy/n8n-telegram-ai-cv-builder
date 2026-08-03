# 🤖 AI-Powered Telegram Resume & CV Builder (n8n Workflow)

An automated, end-to-end micro-SaaS workflow built in **n8n** that converts user messages or uploaded PDF resumes into professionally formatted, ATS-optimized PDF CVs delivered directly inside Telegram.

---

## 🚀 Overview & Architecture

This workflow acts as an intelligent document processing engine. It maintains session state per user, cleans up formatting using an LLM agent, and dynamically generates print-ready A4 PDFs.

### Key Features:
* **Dual Input Pipeline:** Processes both raw Telegram chat messages and uploaded PDF resume files.
* **Persistent User Memory:** Uses Google Sheets keyed by Telegram `chat_id` to allow users to incrementally update their CV over time.
* **AI Formatting Engine:** Utilizes an LLM agent with structured output parsing to fix grammar, rewrite experience into action-oriented bullet points, and normalize skill tags.
* **Custom CSS Rendering:** Converts structured JSON into a clean two-column HTML layout with skill badges, optimized specifically for A4 page dimensions.
* **Automated PDF Delivery:** Converts HTML to binary PDF files via API and posts the finished document directly back to the user's Telegram chat.

---

## 🛠️ Tech Stack & Workflow Nodes

* **Automation Platform:** n8n (LangChain Agent, Code Nodes, HTTP Request)
* **Messaging Interface:** Telegram Bot API
* **Database & Memory:** Google Sheets API
* **AI Model:** OpenAI GPT Model + Structured Output Parser
* **PDF Conversion Engine:** PDFShift API

---

## 📥 How to Import & Use

1. Download the `Telegram CV Bot.json` file from this repository.
2. In your n8n instance, click **Workflows** -> **Import from File**.
3. Configure your API Credentials:
   * **Telegram API:** Enter your Telegram Bot Token.
   * **Google Sheets API:** Connect your OAuth2 account.
   * **PDFShift API:** Add your API Key under HTTP Header / Basic Auth.

---

## 📊 Visual Demo & Output

*(Upload your screenshots here: n8n workflow canvas screenshot, Telegram bot interaction, and sample generated PDF).*
