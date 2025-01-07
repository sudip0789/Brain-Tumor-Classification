# Brain Tumor Classification Using PyTorch

## Overview

This repository demonstrates the use of deep learning for classifying brain MRI scans into four categories:
- **Pituitary Tumor**
- **No Tumor**
- **Meningioma Tumor**
- **Glioma Tumor**

The project leverages state-of-the-art pre-trained models from the TIMM library to achieve high accuracy and efficiency. Various configurations of optimizers, schedulers, and data augmentation techniques are explored to optimize model performance.

## Dataset and Preprocessing

### Dataset
The dataset includes:
- **Training Set**: 2,850 images.
- **Testing Set**: 388 images.

### Preprocessing Steps
- Images resized to `(224, 224)`.
- Converted to tensors and normalized.
- Data augmentation techniques applied:
  - Random flipping, rotation, brightness/contrast adjustment, and grayscale conversion.
  - Advanced augmentations like `AutoAugment` and `RandomResizedCrop`.


## Model Architectures

The following pre-trained models were used:
- **ResNet50**
- **ResNet18**
- **DenseNet121**

Each model's final layer was modified to output predictions for the four classes.

## Training and Testing

### Training
- Loss Function: `CrossEntropyLoss`
- Optimizers: Adam, AdamW, and SGD
- Schedulers: StepLR, CosineAnnealingLR, ExponentialLR
- Techniques: Dropout layers, weight decay.

### Testing
- Metrics: Accuracy, loss, latency, and model size.
- Models evaluated using a separate test dataset.

#### All detailed results and key findings are available in the complete [project report](https://github.com/sudip0789/Brain-Tumor-Classification/blob/main/Brain%20Tumor%20Classification.pdf)
