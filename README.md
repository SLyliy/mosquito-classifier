# Mosquito Classifier

This project focuses on mosquito image classification using deep learning and transfer learning methods. The main goal is to identify mosquito categories from images by comparing the performance of multiple pre-trained convolutional neural network models.

## Project Description

Mosquito recognition is an important image classification task in public health research. Different mosquito species are related to different disease transmission risks, so accurate classification can provide useful support for mosquito monitoring and analysis.

In this project, a transfer learning pipeline was built to classify mosquito images into different classes based on species and condition. Several widely used pre-trained CNN models were selected, trained, and compared under the same experimental setting.

## Objectives

- Build a mosquito image classification system based on deep learning
- Apply transfer learning to improve performance and reduce training time
- Compare multiple pre-trained CNN architectures
- Evaluate model performance using classification metrics and visual results
- Analyze the strengths and weaknesses of different models on this dataset

## Tech Stack

- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## Models Used

- MobileNet
- ResNet50
- VGG16
- InceptionV3

## Dataset

The dataset is organized into multiple classes according to mosquito species and condition. The main categories included in this project are:

- Aedes albopictus landing
- Aedes aegypti landing
- Aedes aegypti smashed
- Aedes albopictus smashed
- Culex quinquefasciatus landing
- Culex quinquefasciatus smashed

These classes allow the models to learn both inter-species differences and visual differences between normal and damaged mosquito samples.

## Repository Structure

```bash
Mosquito Dataset/
└── Mosquito-on-human-skin/
    ├── Aedes albopictus landing/
    ├── Aedes aegypti landing/
    ├── Aedes aegypti smashed/
    ├── Aedes albopictus smashed/
    ├── Culex quinquefasciatus landing/
    ├── Culex quinquefasciatus smashed/
    ├── data_splitting/
    ├── notebook.ipynb
    ├── Report.pdf
    └── README.md
