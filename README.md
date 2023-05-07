# Facial Keypoints Detection

Author: SHAILESH DHAMA
Certainly, here are the detailed steps of the facial keypoints detection project along with statistical formulas in LaTeX style:

### Business problem:
To detect the location of keypoints on face images.

The objective of this project is to predict keypoint positions on face images. This can be used as a building block in several applications, such as:

1. Tracking faces in images and video
2. Analyzing facial expressions
3. Detecting dysmorphic facial signs for medical diagnosis
4. Biometrics / face recognition

### Data
The data can include the source and high-level description (e.g. # obs).

### Steps:

#### Step 1: Data Preprocessing and Cleaning
- Import data and remove missing values.
- Reshape the pixel values to 96x96 size and scale the values to [0, 1].
- Fill missing keypoint values using interpolation.

#### Step 2: Fully Connected Sequential Model
- Build a fully connected sequential model using Keras.
- Compile the model with appropriate loss function and optimizer.
- Fit the model on training data with appropriate batch size and number of epochs.

#### Step 3: Training with Fully Connected Sequential Model
- Train the fully connected sequential model with the training data.
- Evaluate the model on the test data using root mean squared error (RMSE) metric.

#### Step 4: Convolutional Neural Network
- Build a convolutional neural network (CNN) using Keras.
- Compile the model with appropriate loss function and optimizer.
- Fit the model on training data with appropriate batch size and number of epochs.

#### Step 5: Training with Convolutional Neural Network
- Train the CNN model with the training data.
- Evaluate the model on the test data using RMSE metric.

#### Step 6: CNN after Employing Flipped Image Data Generator
- Build a CNN model using Keras with data augmentation using flipped images.
- Compile the model with appropriate loss function and optimizer.
- Fit the model on training data with appropriate batch size and number of epochs.

#### Step 7: Training with CNN(FlippedImage)
- Train the CNN model with flipped image data.
- Evaluate the model on the test data using RMSE metric.

### Results:
- The CNN model output is shown in (./KEYPOINTS_0.png) and the sequential model output is shown in (./KEYPOINTS_1.png).
- The evaluation metrics used to assess model performance are the RMSE between the predicted and actual keypoint locations.

#### RMSE formula:
The root mean squared error (RMSE) is calculated using the following formula:

$RMSE = \sqrt{\frac{1}{N}\sum_{i=1}^{N}(y_{i} - \hat{y_{i}})^{2}}$

where $y_{i}$ is the actual value of the ith keypoint and $\hat{y_{i}}$ is the predicted value of the ith keypoint.

## For Further Information

Please review the narrative of our analysis in [our Jupyter Notebook](./facial-keypoints-detection.ipynb).

For any additional questions, please contact **shaileshshettyd@gmail.com**

## Repository Structure

```
├── README.md                           <- The top-level README for reviewers of this project.
├── facial-keypoints-detection.ipynb    <- Narrative documentation of analysis in Jupyter notebook.
└── images                              <- Both sourced externally and generated from code.
```
