# 📚 Textbook Question Answering using RAG

This project implements a **Retrieval-Augmented Generation (RAG)** pipeline to answer questions from textbook content. It combines dense retrieval (using vector databases like FAISS or Pinecone) with a powerful language model (like GPT or HuggingFace Transformers) to generate accurate, context-aware answers.

---

## 🔧 How It Works

1. **Text Preprocessing**: Textbook content (PDF or text) is chunked into manageable sections.
2. **Embedding & Indexing**: These chunks are embedded using a sentence transformer and stored in a vector database.
3. **Retrieval**: When a question is asked, relevant chunks are retrieved based on vector similarity.
4. **Generation**: Retrieved context is passed to a language model to generate the final answer.

---

## 🚀 Usage

1. Add your textbook file (PDF or text) to the `data/` directory.
2. Run the preprocessing script to split and embed text.
3. Launch the QA pipeline using your preferred interface (CLI, API, or Notebook).

```bash
python main.py --question "What is the law of conservation of energy?"
