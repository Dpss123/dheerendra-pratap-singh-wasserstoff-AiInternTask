# dheerendra-pratap-singh-wasserstoff-AiInternTask

# Wasserstoff AI Internship Task - Document Theme Identifier

A full-stack application that enables document upload, semantic search, and theme synthesis using LLMs (Groq API).

## Tech Stack
- **Frontend:** Streamlit
- **Backend:** FastAPI
- **Database:** ChromaDB (local persistent vector store)
- **OCR & Embedding:** PyMuPDF, PIL, OpenAI Embeddings via Groq
- **LLM Reasoning:** Groq API (GPT-like)

## Features
- Upload multiple PDFs and images
- OCR-based text extraction
- Embedding storage in ChromaDB
- Natural language querying
- Theme synthesis from top document matches


```bash
git clone https://github.com/dheerendra-pratap-singh/wasserstoff/AiInternTask
cd wasserstoff-AiInternTask

# Backend
cd backend
python -m venv venv && source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload

# Frontend
cd ../frontend
streamlit run app.py
