# Neural Network Model Report
Module 21: deep-learning-challenge
## Overview of the Analysis

The non-profit Alphabet Soup is looking to create an algorithm that aids in selecting applicants for funding that have the best chance of success in their ventures. Using my knowledge of machine learning and neural networks, I will use the features in the provided dataset to create a binary classifier the can predict whether applicants will be successful if funded by Alphabet Soup. This analysis involves data preprocessing, model building, training, and evaluation, aiming to achieve a high level of accuracy in classifying the target variable.
 
## Results

* Data Preprocessing:
    * Target Variable: The target variable for the model is 'IS_SUCCESSFUL'
    * Feature Variables: The features for the model include - 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', 'ASK_AMT'
    * Variables to Remove: Drop the 'EIN' and 'NAME' columns due to unique identifier and irrelevent information
 
* Compiling, Training, and Evaluating the Model
    * Number of neurons, layers, and activation functions selected for model:
      * Layers: 3 layers (1 input layer, 2 hidden layers, and 1 output layer)
      * Neurons: First hidden layer: 80 neurons, Second hidden layer: 30 neurons
      * Activation Functions:  ReLU (Rectified Linear Unit) for hidden layers to capture non-linear relationships. Sigmoid for the output layer to produce a probability for binary classification.
    * Target model performance (75%) was not acheived, my model had 72.8% accuracy
    * To increase model performance - I adjusted the number of neurons, dropped additional irrelevant columns, adjusted the number of training epochs, and added more hidden layers.

## Summary

The deep learning model developed for the Alphabet Soup dataset, although falling just shy of our target, demonstrated strong predictive capabilities. The preprocessing steps ensured the input data was clean and relevant, while the model architecture was optimized for performance. *Recommendation:* To further enhance classification performance, it may be beneficial to explore ensemble methods such as Random Forests or Gradient Boosting Machines. These models can capture complex interactions between features and may provide better generalization on unseen data. In addition, they often require less tuning compared to deep learning models and can handle categorical variables more effectively without extensive preprocessing.

