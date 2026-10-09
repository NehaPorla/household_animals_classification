Name : Porla Neha

SRN : PES1UG25AM808

Section : C

# Household Animals Classification Using Deep Learning

Multi-class image classification of animals using transfer learning with **VGG16** and a newer model, **EfficientNetV2B0**, in TensorFlow/Keras.

## Overview
- **Task:** classify an animal photo into one of 10 classes
  (dog, cat, horse, sheep, cow, chicken, elephant, butterfly, spider, squirrel)
- **Dataset:** Animals-10 (Kaggle), split 70% train / 15% validation / 15% test (stratified)
- **Models:** VGG16 (pretrained on ImageNet, frozen base + new top layers) and EfficientNetV2B0 (same approach)
- **Extras:** data augmentation, confusion matrices, feature maps, Grad-CAM heatmaps
- **Reference:** a Stanford-style poster on cats vs dogs classification using VGG models (Lin)

## Method
1. Download the dataset and remove unreadable images
2. Resize to 224 x 224, apply the model-specific preprocessing
3. Augmentation during training: random flip, rotation, zoom
4. Freeze the pretrained base, train new top layers:
   GlobalAveragePooling -> Dense(256, ReLU) -> Dropout(0.5) -> Dense(10, softmax)
5. EarlyStopping on validation loss, evaluation on the untouched test set

## Results
Fill these in from `results/metrics/results.json`.

| Model | Test accuracy | Macro F1 | Training time (min) | Parameters |
|---|---|---|---|---|
| VGG16 (frozen base) | TODO | TODO | TODO | TODO |
| EfficientNetV2B0 (frozen base) | TODO | TODO | TODO | TODO |

Figures (accuracy/loss curves, confusion matrices, Grad-CAM) are in `results/figures/`.

## How to run
1. Open `notebooks/household ani.ipynb` in Google Colab (Runtime -> T4 GPU)
2. Run the cells from top to bottom
3. Paste your Kaggle API token in the hidden box when asked

## Folder structure
```
household-animals-classification/
├── notebooks/   full notebook with outputs
├── data/        dataset instructions (data itself is not committed)
├── models/      model notes / links (files not committed)
├── results/
│   ├── figures/ graphs, confusion matrices, heatmaps
│   └── metrics/ results.json
├── src/         optional scripts
├── requirements.txt
└── README.md
```

## Limitations and future work
- Only 10 classes; an animal outside them is forced into one of the 10
- Some Animals-10 images are mislabelled, which limits the maximum accuracy
- Future: more household animals (rabbit, hamster, bird), a small web demo, fine-tuning

## References
- Animals-10 dataset, Kaggle
- K. Simonyan and A. Zisserman, *Very Deep Convolutional Networks for Large-Scale Image Recognition*, 2014
- M. Tan and Q. Le, *EfficientNetV2: Smaller Models and Faster Training*, 2021
