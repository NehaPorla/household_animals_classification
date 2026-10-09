# Deep Learning Model Development Notebooks

## Project Title
**Household Animals Classification Using Deep Learning: A Comparative Study of VGG16 and EfficientNetB0**

## 1. Overview
This folder contains the Jupyter Notebook used to develop and evaluate a deep learning-based animal image classification system using the Animals-10 dataset. The project compares two convolutional neural network (CNN) architectures, VGG16 and EfficientNetB0, using transfer learning.

The objective is to classify animal images into ten categories and evaluate the performance of both models using appropriate classification metrics and visualizations.

## 2. Notebook Contents

The notebook covers the following stages:

### 2.1 Environment Setup
- Importing the required Python libraries.
- Configuring the deep learning environment in Google Colab.
- Setting up access to the Animals-10 dataset from Kaggle.

### 2.2 Dataset Preparation
- Downloading and extracting the dataset.
- Organizing images into their corresponding animal classes.
- Preparing the dataset for model development.
- Dividing the images into training, validation, and testing subsets.

### 2.3 Image Preprocessing
- Loading images from their class folders.
- Resizing images to the input dimensions required by the models.
- Applying the appropriate preprocessing for each model architecture.
- Preparing batches of images and labels for training and evaluation.

### 2.4 VGG16 Model
VGG16 is a convolutional neural network pretrained on ImageNet. Transfer learning is used by reusing its pretrained feature-extraction layers and adding a classification head for the ten animal categories.

The notebook covers model configuration, training, validation, and performance evaluation.

### 2.5 EfficientNetB0 Model
EfficientNetB0 is another ImageNet-pretrained CNN architecture that uses compound scaling to balance network depth, width, and input resolution.

The notebook applies transfer learning to adapt the pretrained network to the Animals-10 classification task and evaluates its performance.

### 2.6 Model Training
Both architectures are trained and monitored using training and validation metrics. The notebook records the available training history and uses it to examine model learning behaviour.

### 2.7 Model Evaluation
The models are evaluated using relevant classification metrics and visualizations, including:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion matrices
- Training and validation curves, where available

### 2.8 Comparative Analysis
The results from VGG16 and EfficientNetB0 are compared to understand their classification performance on the Animals-10 dataset. The comparison supports an evidence-based assessment of the two architectures.

## 3. Technologies Used
- Python
- TensorFlow and Keras
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Kaggle
- Google Colab
- Jupyter Notebook

## 4. Dataset
The project uses the Animals-10 dataset available on Kaggle:

https://www.kaggle.com/datasets/alessiocorrado99/animals10

The dataset contains ten animal categories: dog, horse, elephant, butterfly, chicken, cat, cow, sheep, spider, and squirrel.

## 5. How to Run
1. Open the notebook in Google Colab.
2. Configure Kaggle access as described in the notebook.
3. Download and prepare the Animals-10 dataset.
4. Run the notebook cells in order.
5. Train the models or load previously saved models if available.
6. Review the evaluation metrics, confusion matrices, and comparison results.

Training time depends on the available hardware and runtime configuration.

## 6. Expected Outcome
The notebook provides an experimental comparison of VGG16 and EfficientNetB0 for multiclass animal image classification. The final results and visualizations are used to assess their relative performance.

## 7. Reproducibility
The notebook documents the workflow from dataset preparation through model evaluation. For reproducibility, use the same dataset split, preprocessing configuration, model settings, and evaluation procedure when comparing results.

---

**Note:** Actual performance values and conclusions should be taken from the completed notebook outputs rather than assumed in advance.
