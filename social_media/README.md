# 📣 Social Media Workflows

This folder contains automation templates for social media engagement and content distribution using n8n, AI, and vector search.

---

## Auto-post Blogs to LinkedIn and Twitter

**Automatically publish blog posts to LinkedIn and Twitter with AI-powered workflow automation.**

### 🚀 What Does This Workflow Do?
- Accepts blog post data via webhook trigger
- Splits and embeds blog content for semantic search
- Stores and queries data in Supabase vector store
- Uses OpenAI for embeddings and Anthropic for content analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from a CMS)
- **Text Splitter:** Prepares blog content for embedding
- **OpenAI Embeddings:** Converts text to vector format
- **Supabase Vector Store:** Stores and queries embeddings
- **Anthropic Chat Model:** Analyzes and summarizes blog content
- **RAG Agent:** Orchestrates retrieval-augmented analysis
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

### 🔑 Required Credentials
- **OpenAI API** (for embeddings)
- **Supabase account** (for vector storage)
- **Anthropic API** (for content analysis)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `auto_blogpost_linkedin_twitter.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (OpenAI, Supabase, Anthropic, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/auto-post-blogs-to-linkedin-and-twitter`) with your blog post data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **OpenAI**: Text embeddings
- **Supabase**: Vector database
- **Anthropic**: LLM content analysis
- **Google Sheets**: Logging
- **Slack**: Alerts

---

## Auto-DM New Twitter Followers

**Automatically send personalized direct messages to new Twitter followers using AI and vector search.**

### 🚀 What Does This Workflow Do?
- Accepts new follower data via webhook trigger
- Splits and embeds follower data for semantic search
- Stores and queries data in Pinecone vector store
- Uses Cohere for embeddings and OpenAI for message generation
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from a Twitter integration)
- **Text Splitter:** Prepares follower data for embedding
- **Cohere Embeddings:** Converts text to vector format
- **Pinecone Vector Store:** Stores and queries embeddings
- **OpenAI Chat Model:** Generates and personalizes DMs
- **RAG Agent:** Orchestrates retrieval-augmented messaging
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

### 🔑 Required Credentials
- **Cohere API** (for embeddings)
- **Pinecone account** (for vector storage)
- **OpenAI API** (for DM generation)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `auto_dm_twitter_new_follower.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (Cohere, Pinecone, OpenAI, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/auto-dm-new-twitter-followers`) with your new follower data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **Cohere**: Text embeddings
- **Pinecone**: Vector database
- **OpenAI**: LLM DM generation
- **Google Sheets**: Logging
- **Slack**: Alerts

---

_Contributions and improvements welcome!_ 