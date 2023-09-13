# Melanoma Detection Using Custom CNN

## Problem Statement

In this assignment, we tackle the critical task of melanoma detection using a custom Convolutional Neural Network (CNN) implemented in TensorFlow. Melanoma is a highly dangerous form of skin cancer, accounting for a significant portion of skin cancer-related deaths. Early detection is crucial for effective treatment and improved patient outcomes. Our objective is to develop a machine learning model capable of accurately identifying melanoma in medical images, assisting dermatologists in their diagnoses and potentially saving lives.

## Assignment Notebook

The Jupyter Notebook containing the assignment tasks and code implementation can be found in repository with the name 'melanoma_detection_assignment.ipynb'.

## Tasks Performed

1. **Data Reading and Understanding**: Initialize the assignment by defining the paths to the training and test images.

2. **Dataset Creation**: Created train and validation datasets from the training directory using a batch size of 32. Ensure that the images are resized to 180x180 pixels.

3. **Dataset Visualization**: Developed code to visualize a sample image from each of the nine classes present in the dataset.

4. **Model Building and Training (First Pass)**: Built a CNN model capable of accurately classifying the nine disease classes. Rescale the images to normalize pixel values between 0 and 1. Choose an appropriate optimizer and loss function. Train the model for approximately 20 epochs. Documented the findings regarding overfitting or underfitting.

5. **Data Augmentation**: Implemented a data augmentation strategy to address potential overfitting or underfitting issues observed in the initial model.

6. **Model Building and Training (Augmented Data)**: Created an augmented dataset and train the CNN model again for approximately 20 epochs. Evaluated whether the issues observed in the initial model have been resolved.

7. **Class Distribution Analysis**: Analyzed the class distribution in the training dataset. Identify the class with the fewest samples and the dominant classes in terms of sample proportions.

8. **Handling Class Imbalances**: Utilize the Augmentor library to rectify class imbalances present in the training dataset.

9. **Model Building and Training (Rectified Data)**: Train a new CNN model on the rectified class imbalance data for approximately 30 epochs. Assess whether the issues identified earlier have been successfully addressed.


## Findings

- By incorporating the Augmentor library, we observed an improvement in training data accuracy.

- Nevertheless, the model continues to exhibit overfitting.

- Addressing the issue of overfitting can be achieved by introducing additional layers, neurons, or incorporating dropout layers.

- Enhancing the model's performance can be achieved through hyperparameter tuning.
