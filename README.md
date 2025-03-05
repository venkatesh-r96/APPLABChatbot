# APPLABChatbot
**Chat bot**

PDF Answering Bot is an AI-powered tool that extracts text from PDFs, generates embeddings for efficient search, and uses GPT-4 to answer user queries based on document content. 
It leverages FAISS for fast retrieval and Sentence Transformers for semantic understanding.

**Setup Instructions**

Install dependencies:
pip install fastapi uvicorn pymupdf openai faiss-cpu numpy sentence-transformers pymupdf python-multipart

**Run the server:**

uvicorn app:app --reload
Access API at http://localhost:8000

**API Endpoints**

POST /upload/ - Upload a PDF
POST /chat/ - Query the chatbot

**Features**

Document-based chatbot using OpenAI API
Fast similarity search using FAISS

**Docker**

Docker deployment check with docker instruction
for docker you need gunicorn
Add that package in requirements.txt

**Conclusion**

This project provides a document-based chatbot using FastAPI, FAISS, and OpenAI GPT-4. It is containerized using Docker and managed using GitHub for version control. 
The API allows users to upload PDFs, extract text, store embeddings, and query the chatbot for relevant answers.
