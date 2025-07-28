# 📝 Content Creation Workflows

## YouTube Transcript to Blog

**Automatically turn YouTube video transcripts into well-structured blog posts using n8n, AI, and vector databases.**

---

### 🚀 What Does This Workflow Do?
- Accepts YouTube transcript data via webhook trigger
- Splits and embeds transcript text for semantic search
- Stores and queries data in Pinecone vector store
- Uses OpenAI for embeddings and Anthropic for blog generation/analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

---

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request
- **Text Splitter:** Prepares transcript for embedding
- **OpenAI Embeddings:** Converts text to vector format
- **Pinecone Vector Store:** Stores and queries embeddings
- **Anthropic Chat Model:** Generates and refines blog content
- **RAG Agent:** Orchestrates retrieval-augmented generation
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

---

### 🔑 Required Credentials
- **OpenAI API** (for embeddings)
- **Pinecone account** (for vector storage)
- **Anthropic API** (for blog generation)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

---

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `youtube2blog.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (OpenAI, Pinecone, Anthropic, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/youtube-transcript-to-blog`) with your transcript data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

---

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **OpenAI**: Text embeddings
- **Pinecone**: Vector database
- **Anthropic**: LLM blog generation
- **Google Sheets**: Logging
- **Slack**: Alerts

---

_Contributions and improvements welcome!_ 