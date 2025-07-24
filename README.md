# RAG-Chatbot
#RAG Q&A Chatbot – Loan Approval Dataset

A Retrieval-Augmented Generation (RAG) chatbot that answers user questions intelligently using a combination of **document retrieval** and **generative AI**. This project leverages sentence embeddings, FAISS for similarity search, and OpenAI (or other available LLMs) to build a contextual question-answering system using the [Loan Approval Prediction Dataset](https://www.kaggle.com/datasets/sonalisingh1411/loan-approval-prediction).

---

## 📌 Features

- 🔍 Document retrieval with **FAISS** + `MiniLM` sentence embeddings  
- 🧠 Generative answering using **OpenAI GPT** (or Claude, Gemini, etc. if credits available)  
- ⚡ FastAPI backend for integration and deployment  
- 🗃️ Works with structured tabular data transformed to natural text  
- 🔄 Easily replaceable embedding models and LLMs  

---

## 🏗️ Project Structure
├── data/
│ └── Training Dataset.csv # Raw data from Kaggle
├── retriever/
│ └── embed_index.py # Embeds & indexes dataset using FAISS
├── llm/
│ └── rag_chain.py # Retrieval and generation logic
├── api/
│ └── main.py # FastAPI backend app
├── requirements.txt # Python dependencies
└── README.md

Example Questions
What is the loan status of applicant 10?

Which applicants were self-employed with graduate education?

What are the income levels of approved applicants?

Tell me about high-income applicants who were rejected.

ech Stack
Python

FastAPI

SentenceTransformers

FAISS

OpenAI / Generative Model

(Optional) LangChain / LlamaIndex / Streamlit

📈 Future Improvements
Add a Streamlit or React frontend interface

Replace OpenAI with Claude, Gemini, or local LLMs

Add chat history and session memory

Deploy to Render / Hugging Face Spaces / Docker

📝 References
Loan Approval Dataset on Kaggle

Sentence Transformers

FAISS – Facebook AI Similarity Search

OpenAI GPT-3.5


