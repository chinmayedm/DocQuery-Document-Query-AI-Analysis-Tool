# DocQuery — Document Query & AI Analysis Tool

DocQuery is a Streamlit-based application that enables users to upload documents and perform AI-powered actions such as summarization, quiz generation, and flash card creation.
It uses a RAG pipeline built with LangChain, HuggingFace embeddings, FAISS, and Groq LLMs.

# 🛠️ Key Features

Upload and process PDF, TXT, or CSV files

Automated document loading and chunking

HuggingFace MiniLM sentence-transformer embeddings

FAISS vector store for fast similarity retrieval

RAG pipeline with Groq models

Three built-in capabilities:

Document Summary

Quiz Generation

Flash Card Creation

# ⚙️ Tech Stack

Component-Technology
Frontend-Streamlit
LLM Provider-Groq (Llama3, Mixtral, Gemma models)
Embeddings-HuggingFace all-MiniLM-L6-v2
Vector Store-FAISS
Framework-LangChain
File Loaders-PyPDFLoader, TextLoader, CSVLoader

# 📂 Supported Document Formats

.pdf

.txt

.csv

# 🚀 How It Works

User uploads a document via the Streamlit sidebar.

The app loads the file using the appropriate LangChain loader.

Text is split into chunks using RecursiveCharacterTextSplitter.

Embeddings are generated using HuggingFace MiniLM.

Chunks are stored in a FAISS index.

A Groq LLM is selected to run a RAG retrieval chain.

Based on user input (Summary / Quiz / Flashcards), the LLM generates output from document context.

# 📦 Installation

Clone the repository and install the required packages:

` pip install -r requirements.txt `

# ▶️ Run the Application

` streamlit run chin.py `

# 📁 Project Structure


# 🧠 Available LLMs (Groq)

Llama3-8b-8192

Llama3-70b-8192

Mixtral-8x7b-32768

Gemma-7b-IT

Gemma2-9b-IT

# 🔐 Note About API Keys

The application requires a valid Groq API key.
Ensure your key is stored securely and not hard-coded in production.
