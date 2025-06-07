# Brain Tumor Detection Using AI

This repository contains a project that leverages Convolutional Neural Networks (CNNs) to classify brain MRI images as either indicating the presence of a tumor (malignant) or not. The project includes steps for building the model, training it on labeled MRI images, and deploying it using Gradio for interactive usage.

---

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Deployment with Gradio](#deployment-with-gradio)
- [Results](#results)
- [Future Work](#future-work)
- [Acknowledgments](#acknowledgments)
- [License](#license)

---

## Project Overview

Brain tumors can be life-threatening and detecting them early is crucial for effective treatment. This project focuses on using machine learning techniques to assist in the classification of brain tumors from MRI scans. The model is designed to classify MRI images into two categories:

- **NO**: No tumor present
- **YES**: Tumor present

The solution also includes an interactive Gradio-based application for real-time predictions.

---

## Dataset

The dataset used in this project is the [Brain MRI Images for Brain Tumor Detection](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection) dataset. It contains MRI images divided into two categories:

- **NO**: MRI scans without a tumor, labeled as `0`  
  <img src="https://brainchangers.thewest.com.au/beating-depression/assets/owbMMgSKx3/mri_0001_11-2083x1906.jpeg" alt="No Tumor MRI" width="200"/>

- **YES**: MRI scans with a tumor, labeled as `1`  
  <img src="https://th.bing.com/th/id/OIP.3xFhX87fwTlBLOlADBrmWQHaH3?w=236&h=220&c=11&rs=1&qlt=90&bgcl=ececec&o=6&pid=PersonalBing&p=0" alt="Tumor MRI" width="400"/>



### Data Details
- Image dimensions: \(240 \times 240\)
- Format: JPEG/PNG
- Classes: Binary (Tumor/No Tumor)

---

## Model Architecture

The machine learning model is built using a Convolutional Neural Network (CNN). The architecture includes the following layers:

1. **Convolutional Layers**: Extract spatial features from images.
2. **MaxPooling Layers**: Reduce spatial dimensions and computational complexity.
3. **Flattening Layer**: Converts 2D feature maps into a 1D feature vector.
4. **Dense Layers**: Fully connected layers for classification.
5. **Dropout Layers**: Prevent overfitting by randomly dropping nodes.

### Libraries Used
- `TensorFlow/Keras` for model building
- `Scikit-learn` for preprocessing
- `Matplotlib` for visualizations
- `Gradio` for deployment

---


### Prerequisites
Ensure you have Python (>= 3.8) installed. Install the required libraries using the following command:

```bash
pip install -r requirements.txt
