# 🧠 Brain Tumor Detection using Deep Learning

A deep learning project for binary classification of brain MRI images into **tumor** and **no-tumor** classes using PyTorch and CNN-based models.

## 📌 Project Overview

This project implements an end-to-end medical image classification pipeline covering:

* Data validation and preprocessing
* Exploratory data analysis
* Image processing with OpenCV
* CNN model development
* Transfer learning with ResNet-18
* Model evaluation
* Grad-CAM-based model interpretability

The dataset contains approximately **3,000 MRI images**, with around 1,500 images in each class.

## 🔄 Project Pipeline

```text
MRI Images
    ↓
Data Validation
    ↓
Image Preprocessing
    ↓
Exploratory Data Analysis
    ↓
CNN Models
    ↓
Model Evaluation
    ↓
Grad-CAM Explainability
```

## 🧹 Data Preprocessing

The preprocessing pipeline includes:

* Checking for valid/corrupted images
* Standardizing image orientation
* Resizing images
* Converting images to grayscale
* Normalizing pixel values
* Data augmentation for model training

Images are processed to a consistent input size of **224 × 224**.

## 🤖 Models

The project explores multiple CNN-based approaches:

### Custom CNN

A convolutional neural network developed for the binary classification task.

### Advanced CNN

A deeper CNN architecture with additional layers for improved feature learning.

### ResNet-18

Transfer learning using a pretrained ResNet-18 model, adapted for grayscale MRI images and two-class classification.

## 📊 Model Evaluation

Models are evaluated using:

* Accuracy
* Confusion matrix
* Classification report
* ROC curve
* Precision-Recall analysis
* Training and validation curves

The notebook compares model behavior across training and validation data.

## 🔍 Explainability with Grad-CAM

Grad-CAM (Gradient-weighted Class Activation Mapping) is used to visualize image regions that contribute to the model's predictions.

This provides a visual interpretation of the model's decision rather than relying only on the classification output.

```text
MRI Image
    ↓
CNN / ResNet-18
    ↓
Prediction
    ↓
Grad-CAM
    ↓
Highlighted Important Regions
```

## 🛠️ Technologies

* Python
* PyTorch
* Torchvision
* OpenCV
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* Grad-CAM

## 📁 Project Structure

```text
brain-tumor-detection-cnn-pytorch/
│
├── notebooks/
│   └── Brain_Tumor_Detection_PyTorch.ipynb
│
├── README.md
└── requirements.txt
```

## 🚀 How to Run

The notebook was developed using Google Colab with GPU acceleration.

1. Clone the repository.
2. Install the required Python packages.
3. Download/prepare the dataset separately.
4. Update the dataset path in the notebook.
5. Run the notebook from the beginning.

The dataset itself is not included in this repository.

## ⚠️ Disclaimer

This project is developed for **educational and research purposes only**. It is not intended to provide medical diagnosis or replace professional medical advice.

## 👩‍💻 Project Scope

This project covers the complete workflow from MRI image preprocessing and model training to evaluation and model explainability using Grad-CAM.
