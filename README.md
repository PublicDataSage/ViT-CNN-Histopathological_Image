# Fusion of Vision Transformer and CNN for Explainable and Efficient Histopathological Image Classification in Cyber-Physical Healthcare Systems

This repository contains code and experiments from the study titled:

**"Fusion of Vision Transformer and Convolutional Neural Network for Explainable and Efficient Histopathological Image Classification in Cyber-Physical Healthcare Systems."**

## 📌 Overview

This project evaluates three deep learning models—CNN, Vision Transformer (ViT), and a hybrid ViT+CNN architecture—on the BreakHis dataset for breast cancer classification. The focus is on achieving a balance between classification accuracy, computational efficiency, and deployment feasibility in cyber-physical healthcare systems.

## 🧪 Models Implemented

- **CNN**: A lightweight convolutional neural network optimized for low-latency environments.
- **ViT**: A transformer-based model capturing global features using self-attention.
- **ViT+CNN**: A hybrid model combining local feature extraction (CNN) and global attention (ViT).

## ⚙️ Training & Evaluation

- Dataset: BreakHis (binary classification: benign vs. malignant)
- Loss Function: `CrossEntropyLoss`
- Optimizer: `Adam`
- Batch Size: 256
- Epochs: 10
- Metrics: Accuracy, Precision, Recall, F1-score
- Evaluation on: `CPU`, `CPU-Edge`, `GPU`, and `GPU-Edge` scenarios

## 📈 Benchmarking

Models are benchmarked for:
- **Inference latency** (sec/image)
- **Memory usage** (MB)
- Plots are generated to visualize model efficiency across deployment environments.

## 🔍 Explainability

Grad-CAM is applied to provide visual explanations for CNN and ViT+CNN predictions to enhance model transparency in medical decision-making.

## 📁 Files

- `Combined.ipynb`: Main notebook containing data loading, model definitions, training loop, evaluation, and benchmarking.
- `README.md`: Project documentation.
