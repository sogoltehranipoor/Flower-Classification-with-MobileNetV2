# Flower-Classification-with-MobileNetV2
Transfer learning image classifier for the Oxford 17 Category Flower Dataset, trained in Google Colab.

## Overview
- Base model: MobileNetV2 (ImageNet weights, frozen)
- Added layers: GlobalAveragePooling2D → Dense(128, ReLU) → Dense(17, Softmax)
- Dataset: [Oxford 17 Flowers](https://www.kaggle.com/datasets/saidakbarp/17-category-flowers) via KaggleHub
- Framework: TensorFlow / Keras

## Workflow
1. Download dataset from Kaggle using `kagglehub`
2. Extract and restructure raw images into 17 class folders
3. Load data with an 80/20 train/validation split
4. Train the classifier for 10 epochs
5. Upload a new image in Colab to get a live prediction

## Results
- Training/validation accuracy and loss plots are generated during training (see notebook output)

## How to run
Open `flowers_colab.ipynb` in Google Colab, set runtime to GPU, and run cells top to bottom.
