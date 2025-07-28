# 📊 Analytics Workflows

## Competitor Price Scraper

**Automate the process of tracking and analyzing competitor pricing using n8n, AI, and vector databases.**

---

### 🚀 What Does This Workflow Do?
- Scrapes competitor pricing data via webhook trigger
- Splits and embeds text for semantic search
- Stores and queries data in Supabase vector store
- Uses OpenAI for embeddings and Anthropic for chat/analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

---

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request
- **Text Splitter:** Prepares data for embedding
- **OpenAI Embeddings:** Converts text to vector format
- **Supabase Vector Store:** Stores and queries embeddings
- **Anthropic Chat Model:** Processes and analyzes data
- **RAG Agent:** Orchestrates retrieval-augmented generation
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

---

### 🔑 Required Credentials
- **OpenAI API** (for embeddings)
- **Supabase account** (for vector storage)
- **Anthropic API** (for chat/analysis)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

---

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `competitor_price_scrapper.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (OpenAI, Supabase, Anthropic, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/competitor-price-scraper`) with your data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

---

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **OpenAI**: Text embeddings
- **Supabase**: Vector database
- **Anthropic**: LLM chat/analysis
- **Google Sheets**: Logging
- **Slack**: Alerts

---

_Contributions and improvements welcome!_ 