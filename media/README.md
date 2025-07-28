# 📺 Media Workflows

This folder contains automation templates for media analytics and campaign monitoring using n8n, AI, and vector search.

---

## Ad Campaign Performance Alert

**Monitor ad campaign performance and receive alerts using AI-powered automation.**

### 🚀 What Does This Workflow Do?
- Accepts ad campaign data via webhook trigger
- Splits and embeds campaign details for semantic search
- Stores and queries data in Pinecone vector store
- Uses Cohere for embeddings and OpenAI for analysis
- Maintains context with window memory
- Logs results to Google Sheets

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from an ad platform)
- **Text Splitter:** Prepares campaign data for embedding
- **Cohere Embeddings:** Converts text to vector format
- **Pinecone Vector Store:** Stores and queries embeddings
- **OpenAI Chat Model:** Analyzes and summarizes campaign context
- **RAG Agent:** Orchestrates retrieval-augmented analysis
- **Google Sheets Logging:** Appends results for tracking

### 🔑 Required Credentials
- **Cohere API** (for embeddings)
- **Pinecone account** (for vector storage)
- **OpenAI API** (for analysis)
- **Google Sheets account** (for logging)

Set up these credentials in your n8n instance before running the workflow.

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `ad_campain_alert.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (Cohere, Pinecone, OpenAI, Google Sheets).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/ad_campaign_performance_alert`) with your campaign data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs.

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **Cohere**: Text embeddings
- **Pinecone**: Vector database
- **OpenAI**: LLM analysis
- **Google Sheets**: Logging

---

## TV Rating Trend Report

**Analyze and report on TV rating trends using AI and vector search.**

### 🚀 What Does This Workflow Do?
- Accepts TV rating data via webhook trigger
- Splits and embeds rating details for semantic search
- Stores and queries data in Redis vector store
- Uses Hugging Face for embeddings and LLM chat/analysis
- Maintains context with window memory
- Logs results to Google Sheets

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from a ratings provider)
- **Text Splitter:** Prepares rating data for embedding
- **Hugging Face Embeddings:** Converts text to vector format
- **Redis Vector Store:** Stores and queries embeddings
- **Hugging Face Chat Model:** Analyzes and summarizes rating trends
- **RAG Agent:** Orchestrates retrieval-augmented analysis
- **Google Sheets Logging:** Appends results for tracking

### 🔑 Required Credentials
- **Hugging Face API** (for embeddings and chat)
- **Redis account** (for vector storage)
- **Google Sheets account** (for logging)

Set up these credentials in your n8n instance before running the workflow.

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `tv_rating_trents.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (Hugging Face, Redis, Google Sheets).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/tv_rating_trend_report`) with your rating data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs.

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **Hugging Face**: Text embeddings & LLM chat
- **Redis**: Vector database
- **Google Sheets**: Logging

---

_Contributions and improvements welcome!_ 