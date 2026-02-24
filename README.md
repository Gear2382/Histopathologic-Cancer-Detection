# Histopathologic Cancer Detection

This project develops a machine learning solution to identify metastatic cancer in small image patches taken from larger digital pathology scans. The goal is to provide a reliable tool to assist pathologists in detecting cancer cells more efficiently and accurately.

## Table of Contents

* [About the Project](https://github.com/Gear2382/Histopathologic-Cancer-Detection/new/main?filename=README.md#about-the-project)
* [Dataset](https://github.com/Gear2382/Histopathologic-Cancer-Detection/new/main?filename=README.md#dataset)
* [Methodology](https://github.com/Gear2382/Histopathologic-Cancer-Detection/new/main?filename=README.md#methodology)
* [Results](https://github.com/Gear2382/Histopathologic-Cancer-Detection/new/main?filename=README.md#results)
* [Installation](https://github.com/Gear2382/Histopathologic-Cancer-Detection/new/main?filename=README.md#installation)

## About the Project

Histopathologic images are a primary tool used by pathologists to diagnose cancer. However, manually scanning these images is time-consuming and prone to human error. This project utilizes a deep learning approach—specifically Convolutional Neural Networks (CNNs)—to classify image patches as either containing or not containing metastatic tissue.

## Dataset

The project uses the **PatchCamelyon (PCam)** benchmark dataset:

* **Input**: $96 \times 96$ pixel color images.
* **Task**: A binary classification task to identify whether the central $32 \times 32$ pixel region contains at least one pixel of tumor tissue.
* **Scale**: The original dataset contains hundreds of thousands of images, providing a robust foundation for training deep learning models.

## Methodology

The notebook follows a standard machine learning pipeline:

1. **Exploratory Data Analysis (EDA)**: Visualizing the distribution of labels and inspecting sample images to understand the data characteristics.
2. **Preprocessing**: Normalizing pixel values and applying data augmentation techniques (like rotation and flipping) to improve model generalization.
3. **Model Architecture**: Implementation of a Convolutional Neural Network (CNN) tailored for image classification.
4. **Training**: Using optimized loss functions and training schedules to achieve high accuracy.
5. **Evaluation**: Measuring performance using metrics like Accuracy and the Area Under the ROC Curve (AUC).

## Results

The model demonstrates high sensitivity and specificity in detecting cancerous regions, significantly reducing the potential workload for medical professionals by highlighting areas of concern.

## Installation

To run the notebook locally, ensure you have the following dependencies installed:

```bash
pip install numpy pandas matplotlib tensorflow keras opencv-python

```

1. Clone the repository:
```bash
git clone https://github.com/Gear2382/Histopathologic-Cancer-Detection.git

```


2. Open the Jupyter notebook:
```bash
jupyter notebook histopathologic-cancer-detection.ipynb

```
