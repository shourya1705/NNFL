# Hand Gesture Recognition Using an Adapted CNN with Data Augmentation

This repository contains the code to implement the paper "Hand Gesture Recognition Using an Adapted CNN with Data Augmentation". The paper is based on Peru sign language. We have implemented it for the American Sign language.

## Dataset Attributes
- Number of Classes = 29
- 1499 images for each class
- Varied Illumination
- Size = 200x200 initially, to be reduced to 128x96
- Training set images = 39150
- Validation set images = 4321
- Testing set = New 300 images

## APIs and Libraries Used
- Keras API
- Tensorflow
- Sklearn
- Matplotlib

## CNN Training Process
- Combination of Back Propagation with Stochastic Gradient Descent.
- Cost of function = Categorical Cross Entropy Loss Function
- Adam Optimizer as optimization function
- Number of Epochs = 10

## Proposed ADCNN
- Performance of baseline CNN is improved by tuning parameters to include kernel initialization and regularization.
- Network Initialization
  - Uniform ‘He Initialization’ for ReLU layers (he_uniform)
  - Uniform ‘Xavier Initialization’ for output softmax (glorot_uniform)
- We have used Kernel regularizer L2 for ReLU layers.

## Results
- Baseline CNN Accuracy
  - Training Set Accuracy = 91.45%
  - Validation Set Accuracy = 69.41%
  - Test Set Accuracy = 60%
- Proposed ADCNN Accuracy
  - Training Set Accuracy = 94.14%
  - Validation Set Accuracy = 72.23%
  - Test Set Accuracy = 62%
Precision, Recall and F-1 Score have been given in the slides

## References
- Research Paper - https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8392660
- Dataset - https://www.kaggle.com/grassknoted/asl-alphabet

## Instructions to Run
    
    git clone https://github.com/shourya1705/NNFL.git
    cd NNFL
    jupyter notebook

Open up `Gesture_BaselineCNN.ipynb` and `Gesture_ADCNN.ipynb` to run the respective models
