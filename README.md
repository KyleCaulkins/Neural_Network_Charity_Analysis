# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to help a data scientist at **Alphabet Soup** build a model that can vet honest non-profits for financial support. Alphabet Soup is a large nonprofit organization that financially backs other nonprofit who help the environment, improve people's wellbeing, and unify the world. Unfortunately, some of the recipient organizations accept donations and then disappear. There is a need to predict which organizations are worth donating to and which are too high risk. The solution needs to be mathematical, data driven, and predict worthy organizations accurately. The following analysis is an attempt to meet this demand using deep learning.  

## Results

### Data Preprocessing

* The data used for processing is in a flat file found [here.](/charity_data.csv)

* The target variable for the deep learning model: *IS_SUCCESSFUL* 

* The features for this model: *APPLICATION_TYPE*, *AFFILIATION*, *CLASSIFICATION*, *USE_CASE*, *ORGINIZATION*, *STATUS*, *INCOME_AMT*, *SPECIAL_CONSIDERATIONS*, *ASK_AMT*

* Variables that are not targets or features for this dataset are: *EIN*, *NAME*. These identifiers do not contribute to the analysis and are removed. 

### Compiling, Training, and Evaluating the Model

* The neural network for this analysis uses a sequential model from the Keras library supported by TensorFlow backend. The model uses a total of three layers, two hidden and one output. There are 80 neurons in the first hidden layer and 30 neurons in the second hidden layer. 80 neurons were selected because is is a rounded double of the input features, and 30 neurons was selected because it is a rounded third of the first hidden layer. This is one of many "rules of thumb" to try for neural architechture. Both hidden layers use the relu activation function, again as a starting rule of thumb. The output layer has a single neuron and a sigmoid activation function because of the desired binary output.

![nn](/challenge/Resources/org_model_layers.png)

* The model
* Were you able to achieve the target model performance?
* What steps did you take to try and increase model performance?

## Summary
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
