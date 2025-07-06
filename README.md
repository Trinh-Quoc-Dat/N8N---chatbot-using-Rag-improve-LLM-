
# 🧠 Chatbot using RAG to Improve LLM Responses (n8n + Supabase + Google Gemini)

## 📖 Overview

This project implements an intelligent chatbot powered by **RAG (Retrieval-Augmented Generation)** on the **n8n** platform. It combines the ability of **Google Gemini (PaLM API)** with **Supabase Vector Store** to enhance the chatbot's response accuracy by retrieving relevant information from your own knowledge base.

⚡ The workflow is fully automated:
- Monitors a Google Drive folder for new or updated files.
- Extracts content from files (currently PDF supported).
- Generates embeddings and stores them in a vector database.
- When a chat message is received, the chatbot performs a semantic search and responds with relevant, enriched answers.

---

## 🛠 Tech Stack

| Technology                | Description                                           |
|---------------------------|-------------------------------------------------------|
| **n8n**                   | Low-code automation platform to build workflows      |
| **Supabase Vector Store** | Vector database for storing and querying embeddings  |
| **Google Gemini (PaLM)**  | Large Language Model for generating embeddings & chat |
| **Google Drive**          | Data source for uploading and managing documents      |

---

## ⚙️ Workflow Highlights

✅ **Google Drive Trigger**: Detects file updates in a specific Drive folder.  
✅ **Download & Extract**: Downloads files and extracts content (PDF supported).  
✅ **Embeddings & Vector Store**: Generates vector embeddings using Google Gemini and stores them in Supabase.  
✅ **Chat Trigger**: Listens for incoming chat messages.  
✅ **AI Agent**: Combines chat history, document search results, and LLM to generate contextual responses.  

---

## 🔧 Prerequisites

- Supabase account with Vector Store setup.
- Google account with:
  - Access to Google Gemini (PaLM) API.
  - Google Drive folder for document storage.
- Configured n8n credentials for:
  - Supabase API
  - Google Gemini (PaLM) API
  - Google Drive API

---

## 🚀 Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/<your-username>/<your-repo>.git
   cd <your-repo>
   ```

2. **Set up n8n:**
   - Import the provided `.json` workflow file into n8n.
   - Configure required credentials in n8n.
   - Activate the workflow.

3. **Test the Workflow:**
   - Upload a document (e.g., PDF) to the configured Google Drive folder.
   - Send a message to the chatbot and observe the enriched, contextual response.

---

## ⚡ Features

- Automatic document ingestion from Google Drive.
- Semantic search with RAG to enhance chatbot responses.
- Simple memory for conversational context.
- Modular design for easy expansion.

---

## 🌱 Future Improvements

- Support for additional file formats (DOCX, TXT, etc.).
- More advanced conversational memory handling.
- Deployment to cloud infrastructure.
- Integration with web or mobile chatbot interfaces.

---

## 🧩 Project Structure

```
├── Chatbot-using-Rag-improve-LLM.json   # n8n workflow export
└── README.md                            # Project documentation
```

---

## 📄 License

This project is licensed under the MIT License.

---

## 🤝 Contributing

Contributions are welcome! Feel free to submit issues or pull requests to improve this project.

---

## 📬 Contact

For questions or collaboration opportunities, please reach out at: [trinhquocdat.02022003@gmail.com]
