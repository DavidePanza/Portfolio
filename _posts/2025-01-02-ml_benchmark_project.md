---
layout: post
title: "ML Algorithm Benchmark"
#date: 2025-01-03
projects: true
description: "Interactive Streamlit app for loading, exploring, and preprocessing datasets with real-time ML algorithm benchmarking"
tag: [machine-learning, streamlit, data-analysis, scikit-learn]
star: false
externalLink: https://github.com/DavidePanza/MLAlgoBench
---

## Project Overview

ML-Models Benchmarker is an interactive Streamlit app that allows users to upload datasets, perform basic preprocessing, and benchmark multiple machine learning algorithms for classification and regression tasks. Supported models include scikit-learn classifiers such as Naive Bayes, Logistic Regression, KNN, LDA, SVM, and Random Forest, as well as LightGBM and CatBoost. Users can explore variable distributions, handle missing values, detect outliers, and perform feature selection, while all visualizations are rendered in real time using Plotly, enabling quick, code-free evaluation of model performance on custom datasets.

### Core Features
- **No-Code Data Analysis**: Load and explore datasets through an intuitive web interface
- **Feature Selection**: Interactive tools for selecting relevant features for model training
- **Model Training**: Support for multiple classification and regression algorithms
- **Real-time Benchmarking**: Compare algorithm performance with live metrics and visualizations

### Data Exploration Tools
- **Data Quality Assessment**: Automated analysis of missing values, data types, and statistical summaries
- **Distribution Visualization**: Interactive plots showing data distributions and patterns
- **Correlation Analysis**: Heatmaps and correlation matrices to understand feature relationships
- **Data Preprocessing**: Built-in tools for handling missing values and feature scaling

### Visualization Features
- **Interactive Charts**: Dynamic visualizations using matplotlib and plotly
- **Model Comparison**: Side-by-side performance comparisons
- **Feature Importance**: Visual representation of feature contributions
- **Learning Curves**: Performance tracking across different dataset sizes

### Technologies Used
- **Frontend**: Python, Streamlit
- **Machine Learning**: Scikit-learn
- **Data Processing**: Pandas, NumPy
- **Visualization**: Matplotlib, Plotly
- **Deployment**: Streamlit Cloud

### Links
- [GitHub Repository](https://github.com/DavidePanza/MLAlgoBench)
- [Try the App](https://davidepanza-mlalgobench-srcmain-cp6iq9.streamlit.app/)