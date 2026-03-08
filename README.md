# Mosquito Classifier

A deep learning image classification project for mosquito recognition using transfer learning models. This project compares multiple pre-trained convolutional neural networks to classify mosquito images by species and condition.

## Project Description

This project explores mosquito image classification in the context of public health research. Different mosquito species are associated with different disease risks, so accurate recognition can support mosquito monitoring and analysis.

A transfer learning pipeline was built to classify mosquito images into multiple categories. Several widely used pre-trained CNN models were selected, trained, and compared under the same experimental setting.

## Objectives

- Build a mosquito image classification system based on deep learning
- Apply transfer learning to improve performance and reduce training time
- Compare multiple pre-trained CNN architectures
- Evaluate model performance using classification metrics and visual results

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
```

## Methodology

This project uses transfer learning as the main training strategy. Pre-trained convolutional neural network models are used as the feature extraction backbone, and a custom classification head is added for the mosquito classification task.

The overall workflow includes:

1. Load and organize the dataset
2. Preprocess images into a suitable input size
3. Select pre-trained CNN models
4. Add classification layers and train the models
5. Validate and compare model performance

## Model Comparison

Several pre-trained CNN architectures were tested in this project:

| Model | Main Characteristic |
|------|----------------------|
| MobileNet | Lightweight and efficient |
| VGG16 | Classic deep CNN structure |
| ResNet50 | Strong feature extraction ability |
| InceptionV3 | Multi-scale feature learning |

## Features

- Multi-class mosquito image classification
- Transfer learning with pre-trained CNNs
- Comparison of multiple deep learning models
- Structured dataset with species and condition labels
- Notebook-based experimental workflow

## Evaluation

The models are mainly evaluated using:

- training accuracy
- validation accuracy
- loss curves
- comparative performance between models

Detailed experimental discussion and result interpretation are included in the project report.

## Files Included

### `notebook.ipynb`

This file contains the main implementation of the project, including data preparation, model construction, training, and evaluation.

### `Report.pdf`

This file contains the written project report, including background, methodology, experiments, results, discussion, and conclusion.

## How to Run

### 1. Install dependencies

```bash
pip install tensorflow keras numpy matplotlib notebook
```

### 2. Start Jupyter Notebook

```bash
jupyter notebook
```

### 3. Open the project notebook

Open `notebook.ipynb` and run the cells step by step.

## Conclusion

This project demonstrates the practical use of transfer learning for mosquito image classification and provides a clear comparison of different CNN architectures on the same dataset.

