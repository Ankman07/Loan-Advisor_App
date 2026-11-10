# Loan Advisor (learning project)

A from-scratch project to learn **ML models**, **RAG chatbots**, and **agents**,
using loan eligibility as the running example.

The original Node/Express + Vite scaffold is preserved untouched in [`legacy/`](legacy/).

## Roadmap

1. **ML model** (`src/ml/`) - load a loan dataset, explore it in `notebooks/`, train and evaluate a classifier (scikit-learn), save it.
2. **RAG chatbot** (`src/rag/`) - embed loan policy/FAQ documents, store them in a vector store, retrieve relevant chunks, answer questions with an LLM.
3. **Agent** (`src/agents/`) - give an LLM tools (the eligibility model, the RAG retriever) and let it decide which to call.
4. **Interface** - a small API/UI on top, once the pieces work.

## Layout

```
data/raw/     datasets (not committed)
notebooks/    exploration
src/ml/       model training + prediction
src/rag/      ingestion, retrieval, chat
src/agents/   tool-using agent
tests/
legacy/       previous code, kept for reference
```

## Setup

```
python -m venv .venv
.venv\Scripts\activate
pip install -r requirements.txt
copy .env.example .env
```
