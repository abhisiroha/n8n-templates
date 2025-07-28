# 👔 HR Workflows

## New Job Application Parser

**Automatically parse and analyze new job applications using n8n, AI, and vector search.**

---

### 🚀 What Does This Workflow Do?
- Accepts job application data via webhook trigger
- Splits and embeds application details for semantic search
- Stores and queries data in Pinecone vector store
- Uses OpenAI for embeddings and LLM chat/analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

---

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from an application form)
- **Text Splitter:** Prepares application data for embedding
- **OpenAI Embeddings:** Converts text to vector format
- **Pinecone Vector Store:** Stores and queries embeddings
- **OpenAI Chat Model:** Analyzes and summarizes application context
- **RAG Agent:** Orchestrates retrieval-augmented analysis
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

---

### 🔑 Required Credentials
- **OpenAI API** (for embeddings and chat)
- **Pinecone account** (for vector storage)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

---

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `job_application_parser.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (OpenAI, Pinecone, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/new-job-application-parser`) with your application data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

---

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **OpenAI**: Text embeddings & LLM chat
- **Pinecone**: Vector database
- **Google Sheets**: Logging
- **Slack**: Alerts

---

_Contributions and improvements welcome!_ 