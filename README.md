#  GenAI News Retrieval with LangChain FAISS Embedding

A Generative AI-powered News Retrieval System using **LangChain, FAISS, and Embeddings** to perform semantic search over news articles.

This project demonstrates how to build a Retrieval-Augmented pipeline that:
- Loads raw text data
- Splits documents into chunks
- Generates embeddings
- Stores them in FAISS vector database
- Performs similarity-based semantic search

---

##  Project Overview

This system retrieves relevant news content based on user queries using vector similarity search instead of keyword matching.

Example dataset used:
- `nvda_news_1.txt` (NVIDIA stock valuation article)
- `sample_text.csv`
- `movies.csv`

---

##  How It Works

### 1️⃣ Load Data
- Load `.txt` or `.csv` files
- Convert into LangChain `Document` format

### 2️⃣ Split Text
- Use `RecursiveCharacterTextSplitter`
- Break large text into smaller chunks

### 3️⃣ Generate Embeddings
- Convert each chunk into vector embeddings

### 4️⃣ Store in FAISS
- Create FAISS vector index
- Store embeddings for fast similarity search

### 5️⃣ Query & Retrieve
- Embed user query
- Perform similarity search
- Return top-k relevant chunks

---
