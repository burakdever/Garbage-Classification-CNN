# Garbage Classification with CNN

## Overview

A deep learning project implementing a Convolutional Neural Network to classify waste images into six categories: cardboard, glass, metal, paper, plastic, and trash. The model is trained on the [Garbage Images Dataset](https://www.kaggle.com/datasets/zlatan599/garbage-dataset-classification) from Kaggle.

Project Notebook: https://www.kaggle.com/code/burakerturk/garbage-classification-cnn
## Dataset

- **Source**: https://www.kaggle.com/datasets/zlatan599/garbage-dataset-classification
- **Classes**: 6 categories (cardboard, glass, metal, paper, plastic, trash)
- **Split**: 70% training, 15% validation, 15% test (stratified)

## Methodology

### Data Processing
- Image resizing to 128x128 pixels
- Data augmentation (rotation, shifts, flips, zoom, shear)
- Normalization to [0,1] range

### Model Architecture
- 4 convolutional blocks with increasing filters (32→64→128→256)
- Batch normalization and dropout for regularization
- Dense layers for classification

### Training Strategy
- Early stopping to prevent overfitting
- Model checkpointing to save best weights

## Future Improvements

- Hyperparameter optimization
- Transfer learning experiments
- Class balancing techniques
- Ensemble methods
