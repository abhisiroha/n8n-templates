# ⚙️ DevOps Workflows

## GitHub Commit Jenkins

**Automate CI/CD by connecting GitHub commit events to Jenkins jobs, with AI-powered context and logging.**

---

### 🚀 What Does This Workflow Do?
- Listens for GitHub commit events via webhook trigger
- Splits and embeds commit data for semantic search
- Stores and queries commit context in Supabase vector store
- Uses OpenAI for embeddings and LLM chat/analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

---

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from GitHub)
- **Text Splitter:** Prepares commit data for embedding
- **OpenAI Embeddings:** Converts commit messages to vector format
- **Supabase Vector Store:** Stores and queries embeddings
- **OpenAI Chat Model:** Analyzes and summarizes commit context
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
   - In n8n, go to **Import Workflows** and select `github_jenkins.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (OpenAI, Supabase, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/github-commit-jenkins`) with your commit data payload (e.g., from a GitHub webhook).
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