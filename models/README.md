# Trained Deep Learning Models

## Overview
This folder is intended to document the deep learning models used in the **Household Animals Classification Using Deep Learning** project.

The project compares two pretrained convolutional neural network (CNN) architectures using transfer learning: VGG16 and EfficientNetB0.

## 1. VGG16
VGG16 is a convolutional neural network developed by the Visual Geometry Group at the University of Oxford. It uses convolutional layers with small \(3 \times 3\) filters to learn hierarchical image features.

In this project, the pretrained VGG16 network is adapted to classify images into ten animal categories using a task-specific classification head.

## 2. EfficientNetB0
EfficientNetB0 is a convolutional neural network that uses a compound scaling approach to balance network depth, width, and input resolution.

In this project, the pretrained EfficientNetB0 network is adapted through transfer learning for the same ten-class animal image classification task.

## Model Files
If saved model files are available, they may be named:

- `vgg16_animals10.keras`
- `efficientnetb0_animals10.keras`

These files represent the trained models and can be loaded for inference and evaluation.

## Model Comparison
VGG16 and EfficientNetB0 are evaluated using the same classification task. Their performance can be compared using accuracy, precision, recall, F1-score, and confusion matrices, where available in the project results.

## Model Availability
Trained model files may be stored separately in Google Drive because of their size. This repository documents the model architectures and their roles in the project.

Refer to the `notebooks/` folder for the implementation, training workflow, and evaluation procedure.
