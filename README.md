# 🤖 WhatsApp AI Agent

A powerful AI-powered WhatsApp Assistant built using **n8n**, **OpenAI**, **WhatsApp API**, and **PostgreSQL Memory**.

This workflow enables users to communicate with an AI agent directly through WhatsApp using **text messages, voice notes, and images**. The agent understands user inputs, processes them with AI, remembers previous conversations, and sends intelligent responses back to WhatsApp.

---

## 🚀 Features

### 💬 Text Message Support

* Receives text messages from WhatsApp.
* Processes user queries using an AI Agent.
* Generates intelligent and contextual responses.

### 🖼️ Image Analysis

* Accepts image messages from WhatsApp.
* Uses OpenAI Vision capabilities to analyze images.
* Converts image content into meaningful text descriptions.

### 🎤 Voice Message Support

* Receives audio messages.
* Transcribes voice recordings into text.
* Sends transcription to the AI Agent for processing.

### 🧠 Conversation Memory

* Stores chat history using PostgreSQL.
* Maintains conversation context across multiple messages.
* Provides more personalized and natural interactions.

### ⚡ Automated Responses

* Automatically sends AI-generated responses back to WhatsApp.
* No manual intervention required.

---

## 🏗️ Workflow Overview

```text
WhatsApp Message
        │
        ▼
     Webhook
        │
        ▼
      Switch
 ┌──────┼──────┐
 │      │      │
 ▼      ▼      ▼
Text   Image  Audio
 │      │      │
 │      ▼      ▼
 │  Image AI  Speech-to-Text
 │      │      │
 └──────┴──────┘
        │
        ▼
     AI Agent
        │
        ▼
 PostgreSQL Memory
        │
        ▼
 Send Reply to WhatsApp
```

---

## 🛠️ Tech Stack

* n8n
* OpenAI
* WhatsApp Cloud API
* PostgreSQL
* Webhooks
* HTTP Requests
* AI Agent Framework

---

## 📂 Workflow Capabilities

### Text Messages

Users can send normal text messages and receive AI-generated responses.

### Image Understanding

Users can upload images and the AI agent can analyze and describe image content.

### Voice Notes

Users can send voice recordings and receive responses based on the transcribed audio.

### Context Awareness

The system remembers previous conversations using PostgreSQL memory.

---

## ⚙️ Prerequisites

Before running the workflow, make sure you have:

* n8n Instance
* OpenAI API Access
* WhatsApp Business API Access
* PostgreSQL Database
* Required Credentials Configured

---

## 📥 Installation

### 1. Clone Repository

```bash
git clone https://github.com/your-username/whatsapp-ai-agent.git
```

### 2. Open n8n

Login to your n8n instance.

### 3. Import Workflow

* Open n8n Dashboard
* Click **Import Workflow**
* Select `Whatsapp.json`

### 4. Configure Credentials

Add:

* OpenAI Credentials
* WhatsApp API Credentials
* PostgreSQL Credentials

### 5. Activate Workflow

Enable the workflow and configure the WhatsApp webhook.

---

## 📸 Use Cases

* Personal AI Assistant
* Customer Support Bot
* FAQ Automation
* Business Chat Automation
* AI Learning Assistant
* Voice-Based Assistant
* Image Understanding Assistant

---

## 🔮 Future Improvements

* Multi-language support
* Document analysis
* RAG-based knowledge retrieval
* Custom business workflows
* Sentiment analysis
* Appointment booking integration

---

## 👨‍💻 Author

**Sushant Patil**

B.Tech Computer Science Engineering Student

Passionate about AI Agents, Automation, Java Development, Cloud Computing, and Real-World AI Solutions.

---

## ⭐ Support

If you found this project useful:

* Star this repository ⭐
* Fork the project 🍴
* Share your feedback 💡

Happy Automating! 🚀
