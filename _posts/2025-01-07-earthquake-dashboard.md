---
layout: post
title: "ETL for Earthquake Dynamic Dashboard"
#date: 2025-01-07
projects: true
description: "Real-time earthquake monitoring dashboard with automated data ingestion pipeline and interactive visualizations"
tag: [react, aws, fastapi, data-engineering, etl]
star: true
# externalLink: https://lnkd.in/e7uCAZcD
---

## Project Overview

The Earthquake Dynamic Dashboard is a React app for visualizing recent earthquakes on a world map and timeline. Data is ingested daily from the USGS Earthquake API through an automated ETL pipeline built with GitHub Actions, AWS Lambda, and S3, then queried via Athena. A FastAPI proxy connects the React frontend to this pipeline, enabling interactive exploration of earthquake locations and temporal patterns. The project combines automated data ingestion with serverless AWS resources and interactive visualizations to track global seismic activity in near real time.

### Data Flow Architecture

**Daily Ingestion Pipeline:**
GitHub Actions cron job → Lambda → Datasource API → S3

**User Query Pipeline:**
React → FastAPI Proxy → API Gateway → Lambda → Athena → S3 → Frontend

### Frontend
- **React Application**: Interactive user interface with real-time data visualization
- **Plotly Visualizations**: Dynamic charts and maps for earthquake data
- **Hosting**: Deployed on Hugging Face Spaces

### Backend Infrastructure
- **Serverless Architecture**: FastAPI with AWS Lambda and API Gateway
- **Data Storage**: AWS S3 for data lake storage
- **Query Engine**: AWS Athena for SQL-based data analysis
- **Automation**: GitHub Actions for scheduled data ingestion

### Key Features
- Real-time earthquake data monitoring
- Interactive global earthquake maps
- Historical data analysis and trends
- Automated daily data updates
- Serverless scalable architecture

### Technologies Used
- **Frontend**: React, Plotly
- **Backend**: FastAPI, AWS Lambda, API Gateway
- **Data Storage**: AWS S3, AWS Athena
- **Data Source**: USGS Earthquake API
- **Automation**: GitHub Actions
- **Development**: Python, AWS SDK

### Links
- [GitHub Repository](https://lnkd.in/e7uCAZcD)
- [Try the App](https://lnkd.in/exNqCbSM)