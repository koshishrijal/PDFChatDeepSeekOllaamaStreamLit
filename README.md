# PDF Chat with DeepSeek - Proof of Concept

This is a simple Proof of Concept (PoC) demonstrating how to upload a PDF file, process its content, generate embeddings using **DeepSeek LLM**, and perform **retrieval-augmented generation (RAG)** using **FAISS** as a vector store.

## Features
- Upload a PDF file via **Streamlit**.
- Extract text from the PDF using **PyPDFLoader**.
- Generate embeddings with **Ollama (DeepSeek LLM)**.
- Store and retrieve documents using **FAISS**.
- Provide AI-powered answers to user queries based on the PDF content.

## Technologies Used
- **Python**
- **Streamlit** (for UI)
- **LangChain** (for document processing & embedding generation)
- **FAISS** (for vector search)
- **Ollama DeepSeek LLM** (for embeddings and responses)

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/pdf-chat-deepseek.git
cd pdf-chat-deepseek
```

### 2. Set Up Virtual Environment
```bash
python -m venv .venv
source .venv/bin/activate  # On macOS/Linux
.venv\Scripts\activate  # On Windows
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

## Running the Application
Start the **Streamlit** UI:
```bash
streamlit run stream_lit.py
```

This will start a local server at **http://localhost:8501**.

## Usage
1. Upload a PDF file.
2. The system will extract, chunk, and embed the content.
3. Ask a question related to the uploaded PDF.
4. The AI will retrieve relevant chunks and generate an answer.

## File Structure
```
.
├── pdfs/                    # Directory for uploaded PDFs
├── stream_lit.py            # Streamlit UI script
├── main.py                  # Core logic for PDF processing & RAG
├── requirements.txt         # Dependencies
└── README.md                # Project documentation
```

## Example Interaction
```
User: What is the due date of invoice?
AI: ...
```
