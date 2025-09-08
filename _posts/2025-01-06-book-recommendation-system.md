---
layout: post
title: "Book Recommendation System with Full Stack ETL"
#date: 2025-01-06
projects: true
description: "Semantic book recommendation system with automated ETL pipeline and vector search capabilities"
tag: [python, airflow, dbt, fastapi, react, vector-search]
star: true
# externalLink: https://github.com/DavidePanza/Book_recommendation_System
---

## Project Overview

The app is a semantic book recommender that uses vector search to return meaningfully similar books. Book data is collected separately, processed through an ETL pipeline, and converted into embeddings with SentenceTransformers. These embeddings are stored in a vector database, which the FastAPI backend queries based on a user’s search. Results are displayed through a React frontend, making the system a simple interface for exploring books by semantic similarity rather than keywords.

### Data Flow Architecture

**Ingestion Pipeline:**
Airflow → Google Books API → S3 → dbt → Athena

**Vector Processing:**
SentenceTransformers → LanceDB for similarity search

**User Query Pipeline:**
React → FastAPI → LanceDB → Semantic results

### Frontend Applications
- **React App**: Interactive book search interface
- **Dash Analytics Dashboard**: Data visualization and analytics

### Backend Infrastructure
- **Orchestration**: Airflow for automated scraping and deduplication
- **Data Transformation**: dbt transformation pipeline
- **API Layer**: FastAPI with vector similarity search
- **Vector Database**: LanceDB for semantic search capabilities

### Key Features
- Semantic book search using vector embeddings
- Automated data ingestion from Google Books API
- Data deduplication and quality management
- Interactive analytics dashboard
- Scalable ETL pipeline architecture

### Technologies Used
- **Orchestration**: Python, Airflow
- **Data Transformation**: dbt
- **Backend**: FastAPI
- **Frontend**: React, Dash
- **Cloud Storage**: AWS S3, AWS Athena
- **Vector Search**: LanceDB, SentenceTransformers
- **Data Source**: Google Books API

### Links
- [GitHub Repository](https://github.com/DavidePanza/Book_recommendation_System)
- [Try the App](https://huggingface.co/spaces/davidepanza/Book_Recommender_App)