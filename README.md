# VGG16-emotion-classifier
# Transfer Learning with VGG16 for Image Classification

This project utilizes transfer learning on the VGG16 model for image classification in the CK Plus dataset. Transfer learning involves pre-training a neural network on a large and complex dataset, such as ImageNet, and using this pre-trained network for classifying images in a different dataset.

## Description

The VGG16 model is a convolutional neural network pre-trained on ImageNet, with a complex architecture capable of extracting deep features from the images to be classified. Through transfer learning, we can leverage the knowledge accumulated by VGG16 during pre-training on ImageNet and apply it to classify images in the CK Plus dataset.

## CK Plus Dataset

The CK Plus dataset contains a collection of facial images of multiple subjects, with different facial expressions. Each image is associated with a label indicating the type of facial expression present in the image. The goal of the project is to train the VGG16 model to correctly classify facial expressions in images.

## Implementation

To use transfer learning with the VGG16 model, follow these steps:

1. Load the pre-trained VGG16.
2. Freeze the base layers of the VGG16 model to retain the pre-trained knowledge.
3. Add a custom classification layer to the model, tailored to the CK Plus dataset.
4. Train the model using the CK Plus dataset, fine-tuning the parameters of the added classification layer.
5. Evaluate the performance of the model on the test dataset and analyze the results obtained.

## Results

| Epochs|    Train accuracy   | Test accuracy  |   Train time   | Test time |
|-------|---------------------|----------------|----------------|-----------|
| 10    | 86.88%              | 83.05%         | 143.06 s       | 5.33 s    |
| 20    | 95.19%              | 89.49%         | 203.06 s       | 5.33 s    |
| 30    | 96.94%              | 93.56%         | 256.66 s       | 5.33 s    |
| 40    | 99.42%              | 95.93%         | 383.09 s       | 3.81 s    |
| 50    | 99.71%              | 98.31%         | 443.16 s       | 5.34 s    |
