# deep-learning-challenge
Module 21 Challenge

Overview
-The purpose of the analysis was to develop a deep learning model to predict the success of funding applications in Alphabet Soup's data. The goal was to preprocess the data, build and train a neural network, and evaluate its performance to determine its effectiveness in predicting successful applications.

Data Preprocessing

What variable(s) are the target(s) for your model?
  * IS_SUCCESSFUL - indictaed whether an application was successful(1) or unsuccessful(0)

What variable(s) are the features for your model?
  * APPLICATION_TYPE
  * AFFILIATION
  * CLASSIFICATION
  * USE_CASE
  * ORGANIZATION
  * STATUS
  * INCOME_AMT
  * SPECIAL_CONSIDERATIONS
  * ASK_AMT

What variable(s) should be removed from the input data because they are neither targets nor features?
  * EIN
  * NAME

Compiling, Training, and Evaluating the Model

How many neurons, layers, and activation functions did you select for your neural network model, and why?
  * First Hidden Layer - 80 neurons, ReLU activation function
  * Second Hidden Layer - 30 neurons, ReLU activation function
  * Output Layer - 1 neuron, Sigmoid activation function
    Reasons why: This provides a mix of complexity and performance. ReLU activation is used for hidden layers because of its       effectiveness in deep learning models. Sigmoid activation is used for the output layer so we can predict probabilities.
    
Were you able to achieve the target model performance?
  * Accuracy: 0.7292
  * Loss: 0.5560
    This falls just under the expected target model performance of 75%
    
What steps did you take in your attempts to increase model performance?
  * Tried different numbers of neurons and layers
  * Tried different activation functions

Summary

The deep learning model developed for Alphabet Soup achieved an accuracy of 72.92%. It is fairly effective in predicting the success of funding applications. Another approach for trying to solve the classification problem could be to try a Random Forest Classifier, like we talked about in class. They might be able to determine or interpret which features are more important for understanding the key drivers that would indicate successful applications.
