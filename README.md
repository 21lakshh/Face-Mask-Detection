# Face Mask Prediction

This project aims to classify images to determine whether a person is wearing a face mask or not. It leverages image processing techniques and a Convolutional Neural Network (CNN) model with max-pooling layers to achieve high accuracy in both training and validation.

## Features
- **Binary Classification**: Identifies if a person is wearing a mask (`With Mask`) or not (`Without Mask`).
- **Image Processing**: Includes resizing, converting images to RGB format, and scaling for effective training.
- **Deep Learning Model**: Uses a CNN with max-pooling layers for feature extraction and classification.
- **Performance**: 
  - Training Accuracy: **93.24%**
  - Validation Accuracy: **92.23%**

## Table of Contents
- [Data Preprocessing](#data-preprocessing)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Future Improvements](#future-improvements)

## Data Preprocessing
Before training the CNN, the following preprocessing steps are performed on the images:
1. **Resizing**: Images are resized to a uniform dimension for consistent input to the CNN.
2. **RGB Conversion**: Converts images to RGB format if not already in this format.
3. **Scaling**: Pixel values are scaled to the range `[0, 1]` for normalization.

## Model Architecture
The CNN architecture is designed with:
- **Convolutional Layers**: Extract spatial features from images.
- **Max-Pooling Layers**: Down-sample feature maps to reduce dimensionality and computational cost.
- **Fully Connected Layers**: Perform the final classification.

The model is compiled with:
- **Loss Function**: Binary Crossentropy
- **Optimizer**: Adam
- **Metrics**: Accuracy

## Results
The model achieved the following performance:
- **Training Accuracy**: 93.24%
- **Validation Accuracy**: 92.23%

## Future Improvements
- Add multi-class classification to include improperly worn masks.
- Enhance the dataset with more diverse images to improve generalization.
- Optimize the model for real-time predictions using lightweight architectures like MobileNet.
