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
```

## Methodology

This project uses transfer learning as the main training strategy. Pre-trained convolutional neural network models are used as the feature extraction backbone, and a custom classification head is added for the mosquito classification task.

The overall workflow includes:

1. Load and organize the dataset
2. Preprocess images into a suitable input size
3. Select pre-trained CNN models
4. Freeze or partially fine-tune the convolutional base
5. Add dense classification layers
6. Train models on the training dataset
7. Validate and compare model performance
8. Analyze results with plots and report discussion

## Image Preprocessing

Before training, the images are preprocessed to make them suitable for model input. Typical preprocessing steps include:

- resizing images to a fixed input size
- normalizing pixel values
- preparing train and validation data
- organizing data into class-based folders

These steps help ensure consistency and improve training stability.

## Model Comparison

Several pre-trained CNN architectures were tested in this project. Each model has different characteristics:

| Model | Main Characteristic |
|------|----------------------|
| MobileNet | Lightweight and efficient, suitable for faster training |
| VGG16 | Classic deep CNN with a simple and uniform structure |
| ResNet50 | Deeper residual network with strong feature extraction ability |
| InceptionV3 | Multi-scale architecture for learning richer visual patterns |

By comparing these models, the project evaluates the trade-off between classification accuracy, feature learning ability, and computational efficiency.

## Features

- Multi-class mosquito image classification
- Transfer learning with pre-trained CNNs
- Comparison of multiple deep learning models
- Structured dataset with species and condition labels
- Notebook-based experimental workflow
- Final written report for analysis and discussion

## Evaluation

The models are evaluated using common classification indicators and visual analysis. The project mainly focuses on:

- training accuracy
- validation accuracy
- loss curves
- comparative performance between models

These metrics are used to understand which model performs better on the mosquito classification task and how model complexity affects the final result.

## Results Summary

The experiments show that different pre-trained models produce different classification performance on the mosquito dataset. Lightweight models such as MobileNet provide better efficiency, while deeper models such as ResNet50 generally show stronger feature extraction capability and better classification performance.

Detailed experimental discussion, figures, and result interpretation are included in the project report.

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

Open the following file in Jupyter Notebook:

```bash
notebook.ipynb
```

### 4. Run all cells

Run the notebook cells step by step to reproduce the training and evaluation process.

## Learning Outcomes

Through this project, the following concepts were practiced and strengthened:

- image classification with deep learning
- transfer learning with pre-trained models
- CNN architecture comparison
- dataset organization for supervised learning
- model evaluation and result analysis
- experiment documentation with notebook and report

## Conclusion

This project demonstrates how transfer learning can be applied to a real image classification task in the public health domain. By comparing several well-known pre-trained CNN architectures, the project shows the practical value of deep learning methods for mosquito recognition and provides a useful experimental basis for further improvement and extension.

