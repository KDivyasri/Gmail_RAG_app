# 📧 Chat with Your Gmail Inbox using RAG

An AI-powered Gmail assistant that lets you **ask questions about your inbox using natural language**. Built with Retrieval-Augmented Generation (RAG) to retrieve relevant email content and generate answers using an LLM.

Built with **Python, Streamlit, OpenAI, Embedchain, ChromaDB, and the Gmail API**.

---

## ✨ Features

- 📬 Chat with your Gmail inbox in natural language
- 🔎 Semantic retrieval of relevant email content
- 🤖 AI-generated answers powered by OpenAI models
- ⚡ Fast vector search using ChromaDB
- 🖥️ Interactive UI built with Streamlit
- 🔐 Secure Gmail authentication via OAuth 2.0

**Example queries:**
- *"Summarize my recent emails"*
- *"Any emails about payments?"*
- *"Who emailed me today?"*
- *"Do I have any emails about interviews?"*

---

## 🧠 How It Works

This app follows a standard **RAG (Retrieval-Augmented Generation)** workflow:

1. Gmail emails are fetched using the **Gmail API**
2. Emails are converted into **vector embeddings** using OpenAI
3. Embeddings are stored in a **ChromaDB vector database**
4. When a user asks a question:
   - Relevant email chunks are retrieved from the vector database
   - The **OpenAI LLM** generates an answer using the retrieved context as a prompt

---

## 🏗️ Architecture

```
User Question
    → Streamlit Interface
    → Embedchain Pipeline
    → ChromaDB Vector Database
    → Relevant Email Context
    → OpenAI LLM
    → Generated Answer
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Frontend | Streamlit |
| LLM & Embeddings | OpenAI API |
| RAG Pipeline | Embedchain |
| Vector Store | ChromaDB |
| Email Integration | Gmail API |
| Auth | OAuth 2.0 |
| Language | Python |

---

## ⚙️ Installation

**1. Clone the repository:**

```bash
git clone https://github.com/YOUR_USERNAME/Gmail_RAG_app.git
cd Gmail_RAG_app
```

**2. Install dependencies:**

```bash
pip install -r requirements.txt
```

---

## 🔑 Gmail API Setup

1. Go to the [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project
3. Enable the **Gmail API**
4. Create an **OAuth Client ID** (Desktop App type)
5. Download the credentials file and rename it to `credentials.json`
6. Place `credentials.json` in the **project root folder**

---

## ▶️ Running the App

```bash
streamlit run app.py
```

A browser window will open where you can:

1. Enter your **OpenAI API key**
2. Authenticate with your **Google account**
3. Start chatting with your Gmail inbox

---

## 📁 Project Structure

```
Gmail_RAG_app/
├── app.py
├── requirements.txt
├── README.md
└── .gitignore
```

---

## 🔒 Security

The following files contain sensitive credentials and **must not be committed to GitHub**. Add them to your `.gitignore`:

```
credentials.json
token.json
```

---

## 💡 Future Improvements

- [ ] AI-generated daily email summaries
- [ ] Automatic action item extraction
- [ ] Email topic clustering
- [ ] Semantic email search filters
- [ ] Slack / Teams integration

---

## 📜 Disclaimer

This project is intended for **educational and demonstration purposes only**.
