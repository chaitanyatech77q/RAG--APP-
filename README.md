📘 RAG Application using LangChain, Ollama, and ChromaDB
📌 Overview

This project demonstrates how to build a Retrieval-Augmented Generation (RAG) application using LangChain, Ollama, and ChromaDB.

The system allows users to query information from a PDF document. It retrieves relevant content and generates accurate responses using a language model.

🚀 Features

Load and process PDF documents

Split text into manageable chunks

Generate embeddings using Ollama

Store embeddings in Chroma vector database

Retrieve relevant context using similarity search

Build an intelligent agent to answer user queries

🛠️ Tech Stack

Python

LangChain

Ollama (LLM + Embeddings)

ChromaDB (Vector Database)

PyPDF

📂 Project Workflow
1. Install Required Libraries
pip install langchain-community pypdf
pip install -U langchain-ollama
pip install -U chromadb langchain-chroma langchain
2. Load PDF Document

The PDF is loaded using PyPDFLoader

Example file: Think and Grow Rich

3. Split the Document

Uses RecursiveCharacterTextSplitter

Breaks text into smaller chunks for better processing

4. Generate Embeddings

Uses Ollama Embeddings

Model: llama3.1:latest

5. Store in Vector Database

Chunks are stored in ChromaDB

Enables fast similarity search

6. Retrieve Relevant Context

Custom tool created using LangChain

Fetches top matching document chunks based on query

7. Build AI Agent

Uses LangChain agent

Combines:

LLM

Retrieval tool

Answers user queries using retrieved context

💡 Example Query
"burning desire as a driving force"

The system:

Searches relevant chunks from the PDF

Retrieves context

Generates a meaningful answer

📁 Directory Structure
├── Rag-app.ipynb
├── chroma_db/
├── input_pdf/
└── README.md
⚙️ How to Run

Install dependencies

Add your PDF file

Run the notebook step-by-step

Ask questions based on your document

🔍 Use Cases

Document-based Q&A systems

Knowledge assistants

AI-powered search engines

Study and research tools

📌 Note

You can replace the input PDF with your own documents

Ensure Ollama is running locally for embeddings and LLM

🤝 Contribution

Feel free to modify and extend this project for your own use cases.

📢 Author

Chaitanya (TechWithChay)
Sharing practical AI, ML, and development insights 🚀
