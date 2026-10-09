# Model Evaluation and Results

## 1. Overview
This folder documents the evaluation results and comparative analysis of the two deep learning models used in the **Household Animals Classification Using Deep Learning** project.

The project compares VGG16 and EfficientNetB0 using transfer learning on the Animals-10 dataset.

## 2. Evaluation Metrics
The models are evaluated using the following metrics, where available in the project notebook:

- **Accuracy:** Measures the proportion of correctly classified images.
- **Precision:** Measures how many images predicted as a particular class belong to that class.
- **Recall:** Measures how many images belonging to a class are correctly identified.
- **F1-score:** Provides a balance between precision and recall.
- **Confusion Matrix:** Shows correct and incorrect predictions for each animal category.

## 3. Training and Validation Curves
Training and validation accuracy and loss curves can be used to understand how each model learns over successive epochs.

These curves help assess learning progress, convergence, and potential overfitting.

## 4. Confusion Matrix
The confusion matrix illustrates classification performance across the ten animal categories:

Dog, Horse, Elephant, Butterfly, Chicken, Cat, Cow, Sheep, Spider, and Squirrel.

It helps identify categories that are correctly classified and categories that are frequently confused with one another.

## 5. Comparative Analysis
VGG16 and EfficientNetB0 are compared based on their recorded evaluation metrics and classification results.

The comparison aims to identify differences in classification performance and understand the suitability of each architecture for animal image classification.

## 6. Results Availability
Evaluation graphs, confusion matrices, comparison tables, and other generated visualizations may be stored in this folder when available.

Additional results and implementation details can be found in the Jupyter Notebook under the `notebooks/` folder.

**Note:** Actual metric values and conclusions should be reported from the completed experiments. No performance values are assumed in this document.
