---
layout: post
title: "YAML Model Parser"
#date: 2025-05-01
projects: true
description: "Pip-installable Python framework for building PyTorch neural networks from YAML configuration files, eliminating tedious architecture code"
tag: [machine-learning, pytorch, python, deep-learning]
star: true
# externalLink: https://github.com/DavidePanza/yaml-model-parser
---

## Project Overview

YAML Model Parser is a pip-installable Python framework that enables developers to build PyTorch neural networks from YAML configuration files instead of writing tedious nn.Sequential code. Inspired by YOLOv5's architecture definition system, this tool simplifies model creation by allowing users to define complex architectures through declarative YAML files. The framework supports skip connections, layer repetition, and concatenation patterns, making it easy to experiment with different architectures without modifying code.

### Core Features
- **Declarative Architecture**: Define neural networks using simple YAML syntax
- **Skip Connections**: Built-in support for residual connections and feature concatenation
- **Layer Repetition**: Repeat blocks multiple times without duplicating configuration
- **Pip Installable**: Easy installation via pip from GitHub or local source

### Supported Architectures
- **YOLO-style Layers**: Conv (Conv2d + BatchNorm + SiLU), C3 (CSP Bottleneck), SPPF, Concat, Detect
- **ResNet-style Layers**: ResBlock, SEBlock (Squeeze-and-Excitation), Bottleneck
- **Standard PyTorch**: Linear, BatchNorm, ReLU, Sigmoid, MaxPool, AvgPool, Dropout, Flatten, Upsample

### YAML Format
Each layer follows the format: `[from, repeat, module, args]`
- **from**: -1 (previous layer), layer index, or list for concatenation
- **repeat**: Number of times to repeat the module
- **module**: Layer type (Conv, ResBlock, Linear, etc.)
- **args**: Layer arguments (channels, kernel size, etc.)

### Extensibility
- **Custom Layers**: Easy registration system for adding new layer types
- **Layer Registry**: Register custom modules to use in YAML configurations
- **Modular Design**: Clean separation between parsing logic and layer implementations

### Technologies Used
- **Python**: Core development language (>=3.7)
- **PyTorch**: Deep learning framework (>=1.9.0)
- **PyYAML**: YAML parsing (>=5.4.0)
- **Setuptools**: Package distribution and installation

### Links
- [GitHub Repository](https://github.com/DavidePanza/Model_Parser)
