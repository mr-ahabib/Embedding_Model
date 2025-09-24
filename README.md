# 📚 PDF to FAISS Embedding Index

This project converts PDFs into vector embeddings and stores them in a **FAISS index** for fast similarity search.  
It’s designed for **semantic search**, **Q&A systems**, and **Retrieval-Augmented Generation (RAG)** apps.

---

## 🚀 Features
- Reads all **PDF files** from a folder.
- Splits each page into text chunks (800 characters).
- Generates embeddings using **all-MiniLM-L12-v2** (SentenceTransformers).
- Stores vectors in **FAISS (`faiss.index`)**.
- Saves text chunks + metadata (file name + page number) in **`index.pkl`**.

---

## 📂 Files
- `faiss.index` → FAISS vector index with embeddings.  
- `index.pkl` → Pickle file storing text chunks + metadata.  

---

## ⚙️ Installation
Install dependencies:

```bash
!pip install faiss-cpu sentence-transformers PyMuPDF
