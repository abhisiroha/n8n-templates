# 🏥 Healthcare Workflows

## Appointment WhatsApp Notify

**Automatically send WhatsApp notifications for healthcare appointments using n8n, AI, and vector databases.**

---

### 🚀 What Does This Workflow Do?
- Accepts appointment data via webhook trigger
- Splits and embeds appointment details for semantic search
- Stores and queries data in Supabase vector store
- Uses OpenAI for embeddings and LLM chat/analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

---

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from an appointment system)
- **Text Splitter:** Prepares appointment data for embedding
- **OpenAI Embeddings:** Converts text to vector format
- **Supabase Vector Store:** Stores and queries embeddings
- **OpenAI Chat Model:** Analyzes and summarizes appointment context
- **RAG Agent:** Orchestrates retrieval-augmented generation
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

---

### 🔑 Required Credentials
- **OpenAI API** (for embeddings and chat)
- **Supabase account** (for vector storage)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

---

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `appointment_notification.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (OpenAI, Supabase, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/appointment-whatsapp-notify`) with your appointment data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

---

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **OpenAI**: Text embeddings & LLM chat
- **Supabase**: Vector database
- **Google Sheets**: Logging
- **Slack**: Alerts

---

_Contributions and improvements welcome!_ 