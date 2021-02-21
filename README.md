# Neural_Network_Charity_Analysis

## Overview of the analysis
The purpose of this analysis is to use Machine Deep Learning and neural networks to create a binary classifier capable of predicting whether an applicant will be successful if funded by Alphabet Soup. 

## Results: 

### Data Preprocessing
- The variable considered the target for the model is 'IS_SUCCESSFUl.'
- The variables considered to be features for the model are APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT. 
- The variables EIN & NAME are neither targets, not features; therefore, these were removed.  

### Compiling, Training, and Evaluating the Model

- Since a good rule of thumb is to have two to three times the amount of neurons in the hidden layer as the number of features, this model has 27 neurons for the first layer and 13 neurons for the second layer. The relu activation function is used to identify nonlinear characteristics from the input values. And in the output layer, the sigmoid activation function will help us predict the probability of an organization funded by Alphabet Soup will be successful. 

- The accuracy of the model is lower than 75%; therefore, the model does not achieve the target performance. 

- To try to increase model performance, the following steps were taken:
  - Noisy variable was removed from features (ASK_AMT)
  - Additional neurons were added to hidden layers
  - Additional hidden layers were added
  - The activation functions of hidden layers and output layers were changed for optimization


## Summary 

Looking at the results of our analysis, the learning model achieved a predictive accuracy of around 72% in the first attempt and after following the steps described above to improve its performance. Therefore, since our goal is to have higher accuracy, an SVM could be an alternative model to try due to its ability to outperform the basic neural network, and even deep learning models, in many straightforward binary classification problems. 
