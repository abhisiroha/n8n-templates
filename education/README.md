# 🎓 Education Workflows

## Quiz Auto Grader

**Automatically grade quizzes using AI, vector search, and workflow automation with n8n.**

---

### 🚀 What Does This Workflow Do?
- Accepts quiz submissions via webhook trigger
- Splits and embeds quiz data for semantic search
- Stores and queries data in Pinecone vector store
- Uses Cohere for embeddings and OpenAI for grading/analysis
- Maintains context with window memory
- Logs results to Google Sheets
- Sends error alerts to Slack

---

### 🛠️ Main Features
- **Webhook Trigger:** Start the workflow with a POST request (e.g., from a quiz platform)
- **Text Splitter:** Prepares quiz data for embedding
- **Cohere Embeddings:** Converts text to vector format
- **Pinecone Vector Store:** Stores and queries embeddings
- **OpenAI Chat Model:** Grades and analyzes quiz responses
- **RAG Agent:** Orchestrates retrieval-augmented grading
- **Google Sheets Logging:** Appends results for tracking
- **Slack Alerts:** Notifies on errors

---

### 🔑 Required Credentials
- **Cohere API** (for embeddings)
- **Pinecone account** (for vector storage)
- **OpenAI API** (for grading/analysis)
- **Google Sheets account** (for logging)
- **Slack API** (for alerts)

Set up these credentials in your n8n instance before running the workflow.

---

### 📥 How to Use
1. **Import the Workflow:**
   - In n8n, go to **Import Workflows** and select `quiz_auto_grader.json` from this folder.
2. **Configure Credentials:**
   - Assign your API keys/accounts to the relevant nodes (Cohere, Pinecone, OpenAI, Google Sheets, Slack).
3. **Trigger the Workflow:**
   - Send a POST request to the webhook endpoint (`/quiz-auto-grader`) with your quiz data payload.
4. **Monitor Results:**
   - Check Google Sheets for logs and Slack for error notifications.

---

### 🧩 Tech Stack
- **n8n**: Workflow automation
- **Cohere**: Text embeddings
- **Pinecone**: Vector database
- **OpenAI**: LLM grading/analysis
- **Google Sheets**: Logging
- **Slack**: Alerts

---

_Contributions and improvements welcome!_ 