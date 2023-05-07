# Facial Keypoints Detection

Author: SHAILESH DHAMA

## Business Problem

The objective of this project is to predict the location of keypoints on face images. This task is important for applications such as facial tracking, facial expression analysis, biometrics/face recognition, and medical diagnosis. Detecting facial keypoints is a challenging problem that requires a robust and accurate model.

## Data

The dataset used in this project is not specified in the readme.md file.

## Steps

1. Data Preprocessing and Cleaning: This step involves cleaning and preprocessing the dataset by removing any missing or incorrect data.

2. Fully Connected Sequential Model: A fully connected sequential model is created to predict the location of facial keypoints.

3. Training with Fully Connected Sequential Model: The fully connected sequential model is trained using the preprocessed dataset.

4. Convolutional Neural Network: A Convolutional Neural Network (CNN) is created to predict the location of facial keypoints.

5. Training with Convolutional Neural Network: The CNN is trained using the preprocessed dataset.

6. CNN after employing Flipped Image Data Generator: The CNN is modified by employing a Flipped Image Data Generator to augment the training data.

7. Training with CNN (Flipped Image): The CNN with flipped images is trained using the preprocessed dataset.

## Results

The output of the CNN model and the Sequential model are shown in the images below.

#### CNN model output
![CNN model output](./images/KEYPOINTS_0.png)
> CNN model output

#### Sequential model output
![Sequential model output](./images/KEYPOINTS_1.png)
> Sequential model output

## For Further Information

Please review the narrative of our analysis in [our Jupyter Notebook](./facial-keypoints-detection.ipynb).

For any additional questions, please contact **shaileshshettyd@gmail.com**

## Repository Structure

```
├── README.md                           <- The top-level README for reviewers of this project.
├── facial-keypoints-detection.ipynb    <- Narrative documentation of analysis in Jupyter notebook.
└── images                              <- Both sourced externally and generated from code.
```
