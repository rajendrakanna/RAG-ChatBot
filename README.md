# 🤖 RAG Chatbot with n8n, OpenAI, Pinecone & Gemini

This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** chatbot using the powerful **n8n** workflow automation platform. The chatbot enables intelligent question-answering over custom documents uploaded by users. It integrates **OpenAI for embeddings**, **Pinecone for vector storage**, and **Google Gemini** for natural language generation.

---

## 🔧 Features

- 📤 Upload `.pdf`, `.txt`, or `.md` files via form
- ✂️ Chunk documents using recursive character splitter
- 🧠 Generate vector embeddings using **OpenAI**
- 🗂️ Store & retrieve vectors using **Pinecone**
- 💬 Real-time chat with context-aware answers using **Google Gemini 2.0**
- ⚙️ Fully visual, modular workflow in **n8n**

---

## 🖼️ Workflow Overview

![RAG Chatbot Workflow](./assets/rag_chatbot_workflow.png)

1. **Document Upload**  
   Triggered by form submission → Loads and splits document → Generates embeddings → Stores in Pinecone.

2. **User Query**  
   Triggered by chat message → Retrieves relevant context → Feeds to Gemini → Returns generated answer.

---

## 🛠️ Requirements

- [n8n](https://n8n.io/) (self-hosted or cloud)
- OpenAI API Key
- Pinecone API Key and Index setup
- Google Gemini (PaLM) API access
- LangChain integration enabled in n8n

