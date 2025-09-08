---
layout: post
title: "Jaguar Identification"
#date: 2025-01-05
projects: true
description: "Computer vision app to identify individual jaguars from camera trap images for conservation research"
tag: [computer-vision, pytorch, conservation]
star: true
# externalLink: https://github.com/JaguarIdentification/ml-jaguar-identification
---

## Project Overview

As part of a three-person team, I developed an application to identify individual jaguars from camera trap images for the Jaguar Identification Project, a citizen-science conservation initiative in Brazil's [Pantanal National Park](https://www.pantanaljaguarsafaris.com/).

### Conservation Impact
This project supports wildlife conservation efforts by automating the identification of individual jaguars from camera trap footage, enabling researchers to track population dynamics and behavior patterns in one of the world's most important jaguar habitats.

### Model Development
- **High Accuracy**: Fine-tuned state-of-the-art computer vision models achieving 70% accuracy 
- **Challenging Dataset**: Worked with highly imbalanced dataset comprising 34 individual jaguar exemplars
- **Advanced Techniques**: Utilized transfer learning and model fine-tuning for optimal performance

### Data Curation
- **Dataset Creation**: Curated comprehensive jaguar dataset hosted on Hugging Face
- **Future Competition**: Dataset will be used for upcoming Kaggle competition sponsored by Voxel51
- **Open Science**: Contributing to open-source conservation research

### Technical Architecture
- **Object Detection**: GroundingDINO for precise jaguar detection
- **Segmentation**: SAM2 for accurate image segmentation
- **Feature Extraction**: DINOv2 for robust visual feature representation
- **Deep Learning**: PyTorch framework for model development

### Key Features
- Individual jaguar identification from camera trap images
- Real-time inference capabilities
- Robust performance on challenging wildlife imagery
- Integration with conservation research workflows

### Technologies Used
- **Deep Learning**: Python, PyTorch
- **Computer Vision Models**: GroundingDINO, SAM2, DINOv2
- **Deployment**: Hugging Face Spaces (Gradio)
- **Model Optimization**: Fine-tuning techniques
- **Data Management**: Hugging Face Datasets

### Links
- [GitHub Repository](https://github.com/JaguarIdentification/ml-jaguar-identification)
- [Try the App](https://huggingface.co/spaces/shahabdaiani/jaguar_identification_app)
- [Dataset](https://huggingface.co/jaguaridentification)