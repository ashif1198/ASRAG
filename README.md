# ASRAG

ASRAG is a simple project to learn how **Traditional RAG (Retrieval-Augmented Generation)** works.

This project uses:

- **LangChain** — document processing
- **Sentence Transformers** — create embeddings
- **ChromaDB** — store and search embeddings
- **Groq** — generate answers using an LLM

The notebooks explain the RAG process step by step.

---

## 📂 Project Structure

```text
ASRAG/
│
├── notebook/
│   ├── document.ipynb
│   ├── traditional_rag_pipeline.ipynb
│   └── 1-langchain-document-components.svg
│
├── data/
│   ├── pdf/
│   ├── text_files/
│   └── vector_store/
│
├── main.py
├── requirements.txt
├── pyproject.toml
└── README.md
```

### Important Files

- `document.ipynb` — Learn about LangChain documents and document loaders.
- `traditional_rag_pipeline.ipynb` — Complete RAG pipeline.
- `data/pdf/` — Sample PDF files.
- `data/text_files/` — Sample text files.
- `data/vector_store/` — ChromaDB vector store.
- `main.py` — Currently a placeholder.

---

## 🔄 RAG Workflow

The project follows this flow:

```text
Documents
    ↓
Load Documents
    ↓
Split into Chunks
    ↓
Create Embeddings
    ↓
Store in ChromaDB
    ↓
User Question
    ↓
Search Relevant Chunks
    ↓
Send Context to LLM
    ↓
Generate Answer
```
---

### `traditional_rag_pipeline.ipynb`

Then move to this notebook to learn the complete RAG pipeline:

- Load PDFs
- Split documents
- Create embeddings
- Store embeddings in ChromaDB
- Retrieve relevant documents
- Generate answers using Groq

Run the notebook cells **in order**.

---

## 📌 Project Status

**Status:** Learning / Experimental

Currently, the RAG pipeline is implemented in the notebooks. `main.py` is not yet used to run the complete RAG pipeline.