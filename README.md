# Facial Keypoints Detection

## Table of Contents

- [Overview](#overview)
- [Data](#data)
- [Methodology](#methodology)
- [Results](#results)
- [Additional Information](#additional-information)
- [Repository Structure](#repository-structure)

## Overview <a name="overview"></a>

This project uses deep learning techniques to detect facial key points in images. Facial key points include points around the eyes, nose, and mouth on a face. These key points are valuable for various applications, such as face tracking in images and videos, facial expression analysis, detection of dysmorphic facial signs for medical diagnosis, and face recognition in biometrics.

## Data <a name="data"></a>

The dataset comprises grayscale images of faces, each tagged with the locations of facial key points. It's important to note that some images might have missing key points.

## Methodology <a name="methodology"></a>

The project involves the following steps:

### 1. Data Preprocessing and Cleaning
- Import the dataset and handle missing values.
- Reshape the pixel values to a size of 96x96 and scale the values to a range of [0, 1].
- Fill in missing keypoint values using interpolation.

### 2. Fully Connected Sequential Model
- Construct a fully connected sequential model using Keras.
- Compile the model using an appropriate loss function and optimizer.
- Train the model using the training data with a specified batch size and several epochs.

### 3. Training with Fully Connected Sequential Model
- Train the fully connected sequential model using the training data.
- Evaluate the model performance on the test data using the root mean squared error (RMSE) metric.

### 4. Convolutional Neural Network (CNN)
- Develop a CNN using Keras.
- Compile the model with an appropriate loss function and optimizer.
- Train the model on the training data with a specified batch size and several epochs.

### 5. Training with Convolutional Neural Network
- Train the CNN model using the training data.
- Evaluate the model performance on the test data using the RMSE metric.

### 6. CNN with Flipped Image Data Generator
- Construct a CNN model using Keras and implement data augmentation using flipped images.
- Compile the model with an appropriate loss function and optimizer.
- Train the model on the training data with a specified batch size and the number of epochs.

### 7. Training with CNN (Flipped Image)
- Train the CNN model using the flipped image data.
- Evaluate the model performance on the test data using the RMSE metric.

## Results <a name="results"></a>

The output of the CNN model is available in the image `KEYPOINTS_0.png`, and the output of the sequential model is in the image `KEYPOINTS_1.png`. The model's performance is evaluated using the RMSE between the predicted and actual key point locations.

The RMSE is computed using the formula:


$RMSE = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(y_{i} - \hat{y_{i}})^{2}}$

where \(y_{i}\) is the actual value of the ith keypoint and \(\hat{y_{i}}\) is the predicted value of the ith keypoint.

## Additional Information <a name="additional-information"></a>

For a more detailed explanation of the methodology and results, please look at the [Jupyter Notebook](./facial-keypoints-detection.ipynb).

For any additional questions or inquiries, please get in touch with me at **shaileshshettyd@gmail.com**.

## Repository Structure <a name="repository-structure"></a>

```plaintext
├── README.md                           <- The top-level README for reviewers of this project.
├── facial-keypoints-detection. ipynb    <- Narrative documentation of analysis in Jupyter notebook
└── images                              <- Images both sourced externally and generated from code
```
