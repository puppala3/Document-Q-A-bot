# Document-Q-A-bot
Project Overview
This project implements an AI-powered Document Q&A bot using the Gemma language model via the Groq API. The bot can answer questions based on the content of PDF documents, demonstrating the capabilities of large language models in understanding and extracting information from structured documents.
Features
PDF document ingestion and processing
Vector embedding for efficient document retrieval
Question-answering based on document content
User-friendly interface built with Streamlit
Integration with Google's Generative AI for embeddings
Technologies Used
Python
Streamlit
LangChain
Groq API
Google Generative AI Embeddings
FAISS for vector storage
PyPDF for PDF processing
How It Works
Document Ingestion:
The system loads PDF documents from a specified directory.
Documents are split into smaller chunks for processing.
Vector Embedding:
Google's Generative AI is used to create embeddings for document chunks.
FAISS is used to store these embeddings for efficient retrieval.
User Interaction:
Users input questions through the Streamlit interface.
Question Answering:
The system retrieves relevant document chunks based on the question.
The Gemma model (via Groq API) generates an answer using the retrieved context.
Result Display:
The answer is displayed to the user.
Relevant document chunks can be viewed for transparency.
Implementation Details
Uses LangChain's create_retrieval_chain for efficient document retrieval.
Implements a custom prompt template for focused question-answering.
Utilizes Streamlit sessions to maintain the vector store across interactions.
Setup and Running
Install dependencies: pip install -r requirements.txt
Set up environment variables for API keys (GROQ_API_KEY, GOOGLE_API_KEY)
Place PDF documents in the "./us_census" directory
Run the application: streamlit run app.py
