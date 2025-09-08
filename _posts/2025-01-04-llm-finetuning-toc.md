---
layout: post
title: "LLM Finetuning for TOC Extraction"
#date: 2025-01-04
projects: true
description: "Fine-tuned small LLM to improve extraction of structured Table of Contents from noisy book data"
tag: [llm, finetuning, nlp, data-processing]
star: false
# externalLink: https://github.com/DavidePanza/streamlit_RAG
---

## Project Overview

This project demonstrates how fine-tuning can improve a small language model (0.6B parameters) on the task of extracting structured tables of contents from noisy book data. Using LoRA parameter-efficient fine-tuning, the model learns to convert inconsistent TOC text into clean JSON with titles and page ranges, significantly outperforming the base model. The repository is designed as a step-by-step tutorial, providing detailed explanations of the full fine-tuning pipeline from data preparation to evaluation.

### Data Processing Pipeline
- **Synthetic Data Generation**: Created 15,000 synthetic examples simulating noisy TOC data with formatting errors
- **Data Distillation**: Processed and cleaned TOC data to create high-quality training examples
- **Noise Simulation**: Introduced realistic formatting errors to improve model robustness

### Model Training
- **Base Model**: Qwen3-0.6B instruction-tuned model
- **Training Platform**: Google Colab for accessible experimentation
- **Optimization**: LoRA (Low-Rank Adaptation) with 4-bit quantization for efficient training
- **Performance**: Demonstrated improved extraction of chapter titles and page ranges over base model

### Technical Implementation
- **Parameter-Efficient Training**: Used LoRA to reduce computational requirements
- **Quantization**: 4-bit quantization for memory efficiency
- **Prompt Engineering**: Carefully designed prompts for optimal extraction performance
- **Unsloth Integration**: Utilized Unsloth for streamlined fine-tuning workflow

### Key Achievements
- Successfully improved structured text extraction from noisy inputs
- Demonstrated effective use of synthetic data for model training
- Achieved significant performance gains with minimal computational resources
- Created reusable dataset for TOC extraction tasks

### Technologies Used
- **Model**: Qwen3-0.6B
- **Training**: LoRA, Unsloth
- **Data**: Synthetic data generation techniques
- **Optimization**: 4-bit quantization
- **Development**: Python, prompt engineering

### Links
- [GitHub Repository](https://github.com/DavidePanza/streamlit_RAG)
- [Fine-tuned Model](https://huggingface.co/davidepanza/qwen3-0.6b-instruct-chapter-extraction)
- [Training Dataset](https://github.com/DavidePanza/finetuning_LLM_for_Chapter_Extraction/tree/main/data)