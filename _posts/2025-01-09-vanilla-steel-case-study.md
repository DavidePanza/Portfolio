---
layout: post
title: "Materials Similarity Analysis Case Study"
#date: 2025-01-09
projects: true
description: "Data science case study analyzing supplier data with custom similarity algorithms for procurement recommendations"
tag: [data-science, pandas, scikit-learn, data-analysis, python]
star: true
# externalLink: https://github.com/DavidePanza/case-study
---

## Project Overview

This is a comprehensive data science case study focused on materials analysis and procurement optimization. The project develops custom similarity algorithms to match Request for Quotation (RFQ) entries with optimal supplier materials. Through extensive data cleaning, feature engineering, and similarity analysis, the system provides top-3 material recommendations based on material properties, physical dimensions, and categorical attributes.

### Data Processing Pipeline
- **Multi-Source Integration**: Merged heterogeneous supplier datasets with inconsistent formats and naming conventions
- **Data Quality Engineering**: Implemented systematic outlier detection and correction based on industry research
- **Feature Engineering**: Parsed complex property strings to extract numerical ranges and engineered meaningful features
- **Missing Value Handling**: Applied domain-informed imputation strategies for categorical and numerical variables

### Similarity Analysis Framework
- **Multi-Component Similarity**: Developed weighted similarity scoring across three dimensions:
  - Grade Properties (12 chemical and mechanical features)
  - Categorical Attributes (5 surface and form characteristics)
  - Physical Dimensions (5 measurements with IoU-based range overlap)
- **Custom Metrics**: Implemented Euclidean distance for properties, categorical matching, and Intersection over Union (IoU) for dimensional ranges
- **Performance Optimization**: Refactored from brute-force to vectorized array operations using NumPy broadcasting

### Exploratory Analysis
- **Ablation Studies**: Systematic evaluation of component contributions to clustering quality
- **Weighting Schemes**: Tested multiple configurations ([1,1,1], [3,1,1], [1,3,1], [1,1,3], [6,3,1])
- **Metric Comparison**: Evaluated Euclidean vs Cosine similarity vs IoU for different feature types
- **Clustering Validation**: Visual inspection revealed that grade properties drive material identity

### Key Findings
- **Component Importance**: Material properties proved most discriminative for categorization
- **Dimensional Significance**: Physical dimensions were application-specific rather than intrinsic identifiers
- **Missing Value Patterns**: Consistent patterns suggested informative missingness in categorical features
- **Data Quality Impact**: Domain-informed cleaning significantly improved clustering coherence

### Technologies Used
- **Python**: Core development language
- **Pandas**: Data manipulation and cleaning
- **NumPy**: Vectorized similarity computations
- **Scikit-learn**: Preprocessing and normalization
- **Matplotlib/Seaborn**: Exploratory data visualization
- **Jupyter Notebooks**: Interactive analysis and documentation

### Project Structure
- **Task 1**: Supplier data integration, standardization, and quality assessment
- **Task 2**: RFQ similarity analysis with custom algorithms and procurement recommendations
- **Modular Codebase**: Separate modules for processing, visualization, similarity computation, and reporting

### Links
- [GitHub Repository](https://github.com/DavidePanza/MaterialsAnalysis_CaseStudy/tree/main) 
