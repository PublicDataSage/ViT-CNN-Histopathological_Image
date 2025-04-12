# Fusion of Vision Transformer and CNN for Explainable and Efficient Histopathological Image Classification in Cyber-Physical Healthcare Systems

This repository contains code and experiments from the study titled:

**"Fusion of Vision Transformer and Convolutional Neural Network for Explainable and Efficient Histopathological Image Classification in Cyber-Physical Healthcare Systems."**

---

## 📁 Repository Structure

This project includes two Jupyter notebooks:

### `data_setup_and_preprocessing.ipynb`  
This notebook handles all dataset preparation tasks. It guides you through:
- Downloading the BreakHis dataset from Kaggle
- Unzipping the dataset and locating the `Breast` folder
- Uploading the dataset to Google Drive
- Verifying the structure for later model training

**Use this notebook first** to ensure that your data is correctly uploaded and accessible in your Colab environment.

---

### `Combined.ipynb`  
This is the core notebook for:
- Defining CNN, ViT, and ViT+CNN models
- Training each model on the BreakHis dataset
- Evaluating classification performance (accuracy, precision, recall, F1-score)
- Applying Grad-CAM for visual explainability
- Benchmarking latency and memory usage across CPU, GPU, and edge environments

**Run this notebook after setting up the dataset using the previous notebook.**

---

## 🧾 Dataset Setup Instructions

1. Create a directory in your Google Drive (e.g., `BreakHisDataset`)
2. Download the dataset from [Kaggle - BreakHis Dataset](https://www.kaggle.com/datasets/ambarish/breakhis)
3. Unzip the file and locate the `Breast` folder
4. Upload the `Breast` folder to your Google Drive directory

You will later access this directory from Colab using `drive.mount()`.

---

## 🧪 Models Overview

- **CNN:** Lightweight, fast architecture ideal for edge devices  
- **ViT:** Transformer-based model for global feature learning  
- **ViT+CNN:** Fusion model that integrates local (CNN) and global (ViT) features

---

## ⚙️ Training Details

- Loss Function: CrossEntropyLoss  
- Optimizer: Adam  
- Batch Size: 256  
- Epochs: 10  
- Evaluation after each epoch using accuracy, precision, recall, and F1-score  
- Inference run in evaluation mode with gradient tracking disabled

---

## 📊 Deployment Benchmarking

Each model is evaluated for:
- Latency (seconds per image)
- Memory usage (MB)

Benchmarks are conducted under:
- CPU
- CPU-Edge
- GPU
- GPU-Edge

---

## 🚀 Getting Started

Clone the repository:

```bash
git clone https://github.com/PublicDataSage/ViT-CNN-Histopathological_Image.git
cd ViT-CNN-Histopathological_Image
