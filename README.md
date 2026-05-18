# 🧠 AI Email Support Classifier (n8n)

An automated AI-powered email support agent built with **n8n + LLM (Groq)**.

---

## 🚀 Features

- 📥 Reads incoming emails via IMAP
- 🧠 Classifies emails:
  - Inquiry
  - Complaint
  - Feedback
- 😊 Detects sentiment (Positive / Neutral / Negative)
- ✉️ Generates intelligent replies
- 🔀 Routes emails using Switch logic
- 📤 Sends automated responses via Gmail

---

## ⚙️ Tech Stack

- **n8n** (workflow automation)
- **Groq API** (LLM)
- **Gmail SMTP / OAuth2**
- **IMAP Email Trigger**

---

## 🔄 Workflow Overview

IMAP Email → Extract Data → AI Model → JSON Output → Switch → Send Reply

---

## 📦 Setup Instructions

### 1. Import Workflow

- Open n8n
- Click **Import**
- Upload `workflow.json`

---

### 2. Configure Credentials

Set up the following in n8n:

- IMAP Email credentials
- Gmail OAuth2 credentials
- Groq API key

---

### 3. Activate Workflow

- Toggle workflow to **Active**
- Send a test email to verify

---

## 🧠 AI Output Format

```json
{
  "category": "Inquiry | Complaint | Feedback",
  "sentiment": "Positive | Neutral | Negative",
  "response": "Generated email reply"
}
