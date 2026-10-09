# Dataset Description

## Animals-10 Dataset

This project uses the Animals-10 dataset to develop a household animal image classification system using deep learning. Two transfer learning models, VGG16 and EfficientNetB0, are used to classify images into 10 animal categories and compare their performance.

### Dataset Source
- **Dataset Name:** Animals-10
- **Platform:** Kaggle
- **Dataset URL:** https://www.kaggle.com/datasets/alessiocorrado99/animals10
- **Task:** Multiclass Image Classification
- **Number of Classes:** 10

### Animal Categories
The dataset contains images belonging to the following categories:

1. Dog
2. Horse
3. Elephant
4. Butterfly
5. Chicken
6. Cat
7. Cow
8. Sheep
9. Spider
10. Squirrel

### Data Preprocessing
The dataset images are organized into folders based on their animal categories. Images are preprocessed and resized to meet the input requirements of the deep learning models. The dataset is divided into training, validation, and testing subsets to train the models, tune their performance, and evaluate their classification accuracy.

### Purpose
The dataset is used to train and evaluate VGG16 and EfficientNetB0 using transfer learning. Their performance is compared using evaluation metrics such as accuracy, precision, recall, F1-score, and confusion matrices, where available in the project notebook.

### Dataset Availability
The complete dataset is not included in this GitHub repository because of its size. It can be downloaded from the original Kaggle source. Refer to the project notebook for dataset preparation and model training instructions.
