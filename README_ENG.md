# Capsule Network Implementation for Pneumonia Detection

**Language:** [Bahasa Indonesia](./README.md) | English

## Project Description

This project implements a Capsule Network (CapsNet) model with activation functions for X-ray image classification to detect pneumonia.

The purpose of this research is to apply Deep Learning methods to classify chest X-ray images into two categories: Normal and Pneumonia.

This project is part of an undergraduate thesis conducted as one of the requirements for completing a Bachelor's degree in Mathematics.

## Research Objectives

1. Implement the Capsule Network architecture for X-ray image classification.
2. Apply activation functions to the Capsule Network architecture.
3. Train the model using an X-ray image dataset.
4. Evaluate the model's ability to classify Normal and Pneumonia images.
5. Analyze model performance based on classification evaluation metrics.

## Dataset

This research uses the Chest X-Ray Images (Pneumonia) dataset from Kaggle, provided by Paul Mooney.

The dataset consists of 5,863 images in two categories:

- Normal
- Pneumonia

### Dataset Split

| Dataset | Number of Images |
|---|---:|
| Training | 4,099 |
| Validation | 877 |
| Testing | 880 |
| **Total** | **5,863** |

## Methodology

The research stages include:

1. Dataset collection and preparation.
2. Image preprocessing.
3. Dataset splitting.
4. Capsule Network architecture development.
5. Model training.
6. Model validation.
7. Model performance evaluation.

## Model Architecture

The main components of the model are:

- Convolutional Layer
- Primary Capsule Layer
- Digit Capsule Layer
- Dynamic Routing
- Squash Activation Function
- Margin Loss

## Model Configuration

| Parameter | Value |
|---|---|
| Programming Language | Python |
| Framework | TensorFlow/Keras |
| Image Size | 128 × 128 pixels |
| Color Mode | Grayscale |
| Epochs | 30 |
| Batch Size | 16 |
| Primary Capsule Dimension | 8 |
| Digit Capsule Dimension | 16 |
| Optimizer | Adam |
| Learning Rate | 0.0001 |
| Routing Iterations | 3 |
| Positive Margin (m+) | 0.9 |
| Negative Margin (m-) | 0.1 |
| Lambda | 0.5 |

## Research Results

| Metric | Result |
|---|---:|
| Training Accuracy | 98.13% |
| Validation Accuracy | 96.12% |
| Testing Accuracy | 96.36% |
| Testing Loss | 4.33% |

The model successfully classified 848 out of 880 test images correctly.

The evaluation was performed using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

### Classification Report

| Class | Precision | Recall | F1-Score | Support |
|---|---:|---:|---:|---:|
| Normal | 0.93 | 0.94 | 0.93 | 238 |
| Pneumonia | 0.98 | 0.97 | 0.97 | 642 |

## Technologies Used

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Scikit-learn
- Google Colab

## Repository Structure

```text
capsule-network-pneumonia-detection/
├── notebooks/
│   └── capsule_network_pneumonia.ipynb
├── results/
├── thesis/
├── README.md
├── README_ENG.md
├── requirements.txt
└── LICENSE
```

## Research Documentation

**Thesis Title:**

Implementation of the Capsule Network Model with Activation Functions for X-ray Image Classification in Pneumonia Detection.

**Author:**

Alfredo Raul Adamsyah

**Study Program:**

Bachelor of Mathematics

**Specialization:**

Statistics

**University:**

University of Lampung

## Notes

This project was developed for academic and research purposes. The model is an experimental image classification system and is not a substitute for professional medical diagnosis.

The dataset is not included in this repository. Users must download the dataset separately from its Kaggle source.

## About the Author

**Alfredo Raul Adamsyah**

Bachelor of Mathematics – Statistics Specialization  
University of Lampung

Areas of Interest:

- Data Analysis
- Statistics
- Machine Learning
- Deep Learning
