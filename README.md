# 🤖 Multi-AI Customer Support System

A production-ready Multi-AI Agent workflow built with **n8n** that automates restaurant customer support through specialized AI agents. Instead of using a single AI agent for every task, this project follows a modular architecture where each agent has one responsibility. A Supervisor Agent manages the conversation, routes requests to the appropriate AI agent, and delivers accurate, context-aware responses.

The system combines **RAG (Retrieval-Augmented Generation)**, conversation memory, CRM automation, and tool calling to answer customer questions, process orders, and automatically store confirmed orders.

---

# 🏗️ Architecture

```text
                 Telegram
                     │
                     ▼
             Supervisor Agent
                     │
        ┌────────────┴────────────┐
        ▼                         ▼
 AI Support Agent            CRM Agent
      (RAG)                      │
        │                        ▼
 Supabase Vector Store     Google Sheets
```

The Supervisor Agent acts as the orchestrator, routing each customer request to the appropriate specialized AI agent.

---

# 🚀 Features

- 🤖 Multi-Agent Architecture
- 🧠 Supervisor Agent for intelligent routing
- 📚 RAG-powered Support Agent
- 💬 Arabic customer support
- 🍔 Retrieves menu and prices from Supabase
- 📝 CRM Agent collects customer information
- 📊 Saves confirmed orders to Google Sheets
- 🧠 PostgreSQL conversation memory
- ⚡ Tool Calling between AI agents
- 📱 Telegram Bot integration

---

# ⚙️ Workflow

1. Customer sends a message on Telegram.
2. Supervisor Agent analyzes the request.
3. Restaurant questions are routed to the AI Support Agent.
4. The Support Agent searches the Supabase Vector Store.
5. Order confirmations are routed to the CRM Agent.
6. CRM Agent collects customer information.
7. The confirmed order is automatically saved to Google Sheets.
8. A confirmation message is returned to the customer.

---

# 🤖 AI Agents

### Supervisor Agent
- Manages the conversation.
- Detects customer intent.
- Routes requests to the correct AI agent.

### AI Support Agent
- Uses RAG with Supabase Vector Store.
- Answers menu and pricing questions.
- Never stores customer information.

### CRM Agent
- Collects customer details.
- Confirms orders.
- Saves confirmed orders to Google Sheets.

---

# 🛠️ Tech Stack

- n8n
- OpenAI
- Telegram Bot API
- Supabase Vector Store
- PostgreSQL
- Google Sheets
- AI Agents
- RAG
- Tool Calling
- Prompt Engineering

---

# 📂 Project Structure

```
Multi-AI-Agent/
│
├── Supervisor Agent
├── AI Support Agent (RAG)
├── CRM Agent
├── PostgreSQL Memory
├── Supabase Vector Store
├── Google Sheets
└── Telegram Integration
```

---

# ⚡ Setup

1. Clone the repository.
2. Import the workflow into n8n.
3. Configure OpenAI, Telegram, PostgreSQL, Supabase, and Google Sheets credentials.
4. Activate the workflow.

---

# ▶️ Usage

Ask restaurant questions through Telegram, browse the menu, place an order, and confirm it. The AI automatically retrieves restaurant information using RAG and stores confirmed customer orders in Google Sheets.

---

# 🚀 Future Improvements

- WhatsApp Integration
- Voice AI Assistant
- Stripe Payments
- Delivery Tracking
- Analytics Dashboard
- Inventory Management Agent
- Multi-language Support

---

# 📸 Screenshots

```
screenshots/
│
├── workflow.png
├── supervisor-agent.png
├── support-agent.png
├── crm-agent.png
├── telegram-chat.png
└── google-sheets.png
```

---

# 📄 License

This project is licensed under the **MIT License**.

Feel free to use, modify, and extend this project for learning or commercial purposes.

---

## 👨‍💻 Author

**Abde STAILI**

AI Automation Engineer

Specializing in AI Agents, Multi-Agent Systems, Workflow Automation, n8n, and RAG Applications.
