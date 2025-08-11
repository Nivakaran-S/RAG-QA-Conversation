# Conversational RAG Q&A with PDF Upload & Contextual Chat History

## 🚀 Project Overview

This project is an **advanced Conversational Retrieval-Augmented Generation (RAG) application** built with Streamlit that enables **interactive question answering over uploaded PDF documents** — enhanced with **dynamic chat history awareness** to simulate natural, contextual conversations.

Using state-of-the-art embedding models and Groq’s powerful LLM, this app demonstrates how AI can be combined with custom document ingestion pipelines to deliver precise, contextually relevant answers, making it a perfect showcase of skills in:

- Natural Language Processing (NLP)
- Large Language Models (LLMs)
- Vector Search & Semantic Retrieval
- Conversational AI
- Modern Python development & API integration

---

## 💡 Key Features

- **Multi-PDF Upload:** Seamlessly upload multiple PDF files for simultaneous knowledge ingestion.
- **Robust Document Processing:** Intelligent chunking and semantic embedding using HuggingFace’s `all-MiniLM-L6-v2`.
- **Chroma Vector Store:** High-performance, scalable vector search for lightning-fast context retrieval.
- **Groq LLM Integration:** Leverages Groq’s `Gemma2-9b-It` for advanced question understanding and concise answer generation.
- **Context-Aware Conversations:** Maintains chat history per session to enable follow-up questions and natural dialogue flow.
- **Standalone Question Reformulation:** Automatically transforms ambiguous questions into context-independent queries to maximize retrieval accuracy.
- **User-Friendly Streamlit UI:** Intuitive interface for API key input, document uploads, and live chat interactions.

---

## 🎯 Why This Project?

This mini project encapsulates essential, industry-relevant skills and concepts for AI & Data Science roles:

- Hands-on experience with **retrieval-augmented generation (RAG)** workflows.
- Expertise in **embedding-based semantic search** — crucial for next-gen AI search engines.
- Real-world application of **conversational AI** techniques with **session-aware context management**.
- Practical integration of cutting-edge APIs (Groq LLM, HuggingFace, Chroma).
- Clean, modular, and production-ready **Streamlit app** showcasing end-to-end ML pipeline deployment.

This project is a testament to my ability to engineer scalable AI solutions that combine NLP, vector search, and user experience — perfect for data-driven companies and AI startups.

---

## 📦 Tech Stack

| Technology           | Purpose                               |
| -------------------- | ----------------------------------- |
| Python 3.8+          | Core programming language            |
| Streamlit            | Web UI framework                     |
| LangChain            | LLM & retrieval orchestration        |
| Groq LLM API         | Language model for question answering|
| HuggingFace Embeddings | Semantic vector generation          |
| Chroma Vector Store  | Embedding indexing & retrieval       |
| PyPDFLoader          | PDF ingestion & parsing               |
| dotenv               | Environment variable management       |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- A valid **Groq API Key** (register at [Groq](https://www.groq.com/))
- HuggingFace token (for embedding model access)

### Installation

```bash
git clone https://github.com/yourusername/conversational-rag-pdf-chat.git
cd conversational-rag-pdf-chat

python -m venv venv
source venv/bin/activate  # Windows: .\venv\Scripts\activate

pip install -r requirements.txt
```

### Create a .env file in the project root and add your Huggingface token:
```bash

HF_TOKEN=your_huggingface_token_here

```

### Running the App
```bash

streamlit run app.py

```
- Enter your Groq API key when prompted.
- Upload one or multiple PDF documents.
- Enter a session ID to start a new chat or continue an existing one.
- Ask questions related to the uploaded PDFs and get concise, accurate answers with chat history context.

## 📈 How It Works: High-Level Flow
1. PDF Upload & Parsing: Extracts raw text from PDFs using PyPDFLoader.

2. Text Chunking: Splits documents into overlapping chunks optimized for semantic search.

3. Embedding Creation: Uses HuggingFace’s all-MiniLM-L6-v2 to convert text chunks into vector embeddings.

4. Vector Indexing: Stores embeddings in Chroma for efficient retrieval.

5. Contextual Question Reformulation: Reformulates follow-up questions to standalone queries considering chat history.

6. Relevant Context Retrieval: Retrieves top relevant document chunks via vector similarity search.

7. Answer Generation: Groq LLM generates precise, concise answers using retrieved context.

8. Session-Based Chat History: Maintains history enabling multi-turn conversations with context awareness.

## 🙌 Contributions

--

Contributions and improvements are welcome! Feel free to open issues or submit pull requests.


Thank you for checking out my project! I hope it demonstrates my passion for applied AI and building impactful tools.