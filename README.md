# 🧠 Brain Tumor Detection Using AI

This repository contains a deep learning project that uses **Convolutional Neural Networks (CNNs)** to classify brain MRI images as either indicating the presence of a tumor or not. The project walks through model building, training on labeled data, and deployment using **Gradio** for real-time usage.

---

## 📑 Table of Contents

- [📌 Project Overview](#project-overview)
- [📂 Dataset](#dataset)
- [🧠 Model Architecture](#model-architecture)
- [⚙️ Setup and Installation](#setup-and-installation)
- [🚀 Usage](#usage)
- [🌐 Deployment with Gradio](#deployment-with-gradio)
- [🙏 Acknowledgments](#acknowledgments)
- [📄 License](#license)

---

## 📌 Project Overview

Brain tumors can be life-threatening, and early detection is crucial. This project applies **machine learning** techniques to automate the classification of brain tumors from MRI scans.

The model classifies MRI images into two categories:

- **NO** — No tumor present
- **YES** — Tumor present

A web-based interface built with **Gradio** allows users to test the model interactively.

---

## 📂 Dataset

The dataset used is the [Brain MRI Images for Brain Tumor Detection](https://www.kaggle.com/navoneel/brain-mri-images-for-brain-tumor-detection) from Kaggle. It consists of MRI scans categorized into:

- **NO**: MRI scans **without** a tumor (`label = 0`)  
  <img src="https://brainchangers.thewest.com.au/beating-depression/assets/owbMMgSKx3/mri_0001_11-2083x1906.jpeg" alt="No Tumor MRI" width="300"/>

- **YES**: MRI scans **with** a tumor (`label = 1`)  
  <img src="https://th.bing.com/th/id/OIP.3xFhX87fwTlBLOlADBrmWQHaH3?w=236&h=220&c=11&rs=1&qlt=90&bgcl=ececec&o=6&pid=PersonalBing&p=0" alt="Tumor MRI" width="400"/>

- **Gradio Input Sample Images**:  
  ![Gradio Input Samples](https://github.com/Perwil/Brain_Tumor_Detection_App/blob/main/MRI%20Brain%20images.png)

### 📊 Data Details

- Image dimensions: `240 x 240`
- Format: `.jpg` / `.png`
- Classes: Binary (`Tumor` / `No Tumor`)

---

## 🧠 Model Architecture

The model is built using a **CNN (Convolutional Neural Network)** with the following components:

1. 🧱 **Convolutional Layers** — for spatial feature extraction  
2. 🌀 **MaxPooling Layers** — for dimensionality reduction  
3. 📉 **Flatten Layer** — flattens feature maps to vectors  
4. 🎯 **Dense Layers** — fully connected for classification  
5. 🧪 **Dropout Layers** — to prevent overfitting

<img src="https://github.com/Perwil/Brain_Tumor_Detection_App/blob/main/model_architecture.png" alt="Model Architecture" width="600"/>

### 🧰 Libraries Used

- `TensorFlow` / `Keras` – Model building and training  
- `Scikit-learn` – Preprocessing and evaluation  
- `Matplotlib` – Visualization  
- `Gradio` – Web app deployment

---

## ⚙️ Setup and Installation

Ensure you have Python **3.8+** installed. Then install the required packages:

```bash
pip install -r requirements.txt
