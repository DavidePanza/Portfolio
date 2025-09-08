---
layout: post
title: "Mistral7b RAG"
#date: 2025-01-02
projects: true
description: "RAG tool for uploading, searching, and generating responses from user-provided documents using a quantized Mistral 7B model"
tag: [llm, rag, streamlit, mistral, docker]
star: false
externalLink: https://github.com/DavidePanza/mistral7b-RAG-ui
---

## Project Overview

This project is a Retrieval-Augmented Generation (RAG) tool that allows users to upload documents and query them with a quantized Mistral 7B model. Uploaded documents are processed into embeddings and stored in a temporary in-memory knowledge base, enabling document-specific question answering. 

### Backend Architecture
- **Document Processing**: Support for .txt and .pdf files with automated text extraction
- **Vector Database**: ChromaDB for efficient document indexing and similarity search
- **Language Model**: Quantized Mistral 7B model optimized for performance and resource efficiency
- **RAG Pipeline**: Combines document retrieval with generative AI for contextual responses

### Frontend Interface
- **Streamlit UI**: Clean, intuitive web interface for document upload and querying
- **Interactive Chat**: Real-time conversation interface with document-based responses
- **File Management**: Easy document upload and processing workflow
- **Response Streaming**: Live response generation for better user experience

### Technologies Used
- **Language Model**: Mistral7b-4bit (quantized)
- **Frontend**: Streamlit
- **Vector Database**: ChromaDB
- **Architecture**: RAG (Retrieval-Augmented Generation)
- **Hosting**: RunPod serverless platform
- **Deployment**: Hugging Face Spaces
- **Containerization**: Docker

### Links
- [GitHub Repository](https://github.com/DavidePanza/mistral7b-RAG-ui)
- [Try the App](https://huggingface.co/spaces/davidepanza/Mistral-RAG)