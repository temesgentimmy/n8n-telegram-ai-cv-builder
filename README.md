# 🚀 Telegram AI Resume & PDF Generator (n8n Workflow)

An automated, end-to-end workflow built with **n8n**, **OpenAI**, **Telegram Bot API**, and **PDFShift**. This tool converts unstructured text sent via Telegram into structured JSON, parses it into styled HTML/CSS templates, and delivers a print-ready A4 PDF back to the user in seconds.

---

## 🚧 Project Status & Ongoing Upgrades

> 💡 **Note for Reviewers & Recruiters:** 
> This workflow is actively being maintained and upgraded to commercial grade. 

* **Template Polish:** Fine-tuning line wrapping, spacing, and dynamic element heights (as seen in recent test builds) to ensure zero visual clipping across all text lengths.
* **Cover Letter Generator:** Adding an automated AI pipeline step to generate tailored cover letters based on the user's resume data and job description.
* **Interview Preparation Bot:** Introducing an interactive Telegram feature that generates key interview questions and STAR-method answer prep based on the generated CV.
* **Multi-Template Selector:** Implementing an inline Telegram keyboard allowing users to choose between **Modern**, **Minimalist**, and **Executive** CV designs.

---

## 🛠️ Tech Stack & Architecture

* **Automation Platform:** n8n (Self-Hosted / Cloud)
* **Trigger & Delivery:** Telegram Bot API
* **AI & Data Extraction:** OpenAI API (Structured JSON Parsing)
* **Templating & Rendering:** HTML5, CSS Grid & Flexbox, JavaScript
* **PDF Conversion:** PDFShift API

---

## ⚙️ How It Works


---

## 📥 How to Import & Use

1. Download the `Telegram CV Bot.json` file from this repository.
2. In your n8n instance, click **Workflows** -> **Import from File**.
3. Configure your API Credentials:
   * **Telegram API:** Enter your Telegram Bot Token.
   * **Google Sheets API:** Connect your OAuth2 account.
   * **PDFShift API:** Add your API Key under HTTP Header / Basic Auth.
4. Activate the workflow and test by sending text to your Telegram Bot!

