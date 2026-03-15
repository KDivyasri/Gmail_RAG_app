
# 📧 Chat with Your Gmail Inbox using RAG

An AI-powered Gmail assistant that allows you to **ask questions about your inbox using natural language**.
This project uses **Retrieval-Augmented Generation (RAG)** to retrieve relevant email content and generate answers using an LLM.

Built with **Python, Streamlit, OpenAI, Embedchain, ChromaDB, and the Gmail API**.

---

## 🚀 Features

- 📬 Chat with your Gmail inbox
- 🔎 Semantic retrieval of email content
- 🤖 AI-generated answers using OpenAI models
- ⚡ Vector search using ChromaDB
- 🖥️ Interactive UI built with Streamlit
- 🔐 Secure Gmail authentication using OAuth

Example queries:

- Summarize my recent emails
- Any emails about payments?
- Who emailed me today?
- Do I have emails about interviews?

---

## 🧠 How It Works

This application follows a **Retrieval-Augmented Generation (RAG)** workflow:

1. Gmail emails are fetched using the Gmail API
2. Emails are converted into **embeddings** using OpenAI
3. Embeddings are stored in a **Chroma vector database**
4. When a user asks a question:
   - Relevant email chunks are retrieved from the vector database
   - The LLM generates an answer using the retrieved context

---

## 🏗️ Architecture

User Question
->
Streamlit Interface
->
Embedchain Pipeline
->
Vector Database (Chroma)
->
Relevant Email Context
->
OpenAI LLM
->
Generated Answer

---

## 🛠️ Tech Stack

- Python
- Streamlit
- OpenAI API
- Embedchain
- ChromaDB
- Gmail API
- OAuth2 Authentication

---

## ⚙️ Installation

Clone the repository:

- git clone https://github.com/YOUR_USERNAME/Gmail_RAG_app.git
- cd Gmail_RAG_app

Install dependencies:

pip install -r requirements.txt

---

## 🔑 Gmail API Setup

1. Go to Google Cloud Console
2. Create a new project
3. Enable **Gmail API**
4. Create **OAuth Client ID (Desktop App)**
5. Download the credentials file
6. Rename it to:

credentials.json

Place it in the **project root folder**.

---

## ▶️ Run the Application

Start the Streamlit app:

streamlit run app.py

A browser window will open where you can:

- Enter your **OpenAI API key**
- Authenticate with your **Google account**
- Start chatting with your Gmail inbox

---

## 📁 Project Structure

Gmail_RAG_app/
│
├──app.py
├──requirements.txt
├──README.md
└──.gitignore

---

## 🔒 Security

Sensitive files should not be pushed to GitHub.

Add these to `.gitignore`:

- credentials.json
- token.json

---

## 💡 Future Improvements

- AI-generated daily email summaries
- Automatic action item extraction
- Email topic clustering
- Semantic email search filters
- Slack / Teams integration

---

## 📜 Note

This project is intended for **educational and demonstration purposes**.
