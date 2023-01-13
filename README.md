# Neural_Network_Charity_Analysis
## Overview of the analysis: 
Alphabet Soup receives funding from more than 34, 000 organizations with some being short term while others are more long term funding. Alsphabet Soup wants to create a binary classifier that is able to predict whether applicants will be successful if funded by Alphabet Soup. To determine whether the money was used effectively by deep learning.

## Results: 
### Data Preprocessing
variable target for model  
- IS_SUCCESSFUL

variables features for model
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT
- IS_SUCCESSFUL

Variable are neight targets nor features
- EIN
- NAME

### Compiling, Training, and Evaluating the Model
Initial neural network model:
In the inital neural network model created in AlphabetSoupCharity.ipymb had 2 hidden layers with the first layer having 80 hidden nodes and the second layer having 30 nodes. The activation function for both hidden layers are relu and the activation function for output layer is sigmoid.

Figure 1. The layers of the first neural network model. 
Removed status
- Number of neurons: 110
- Number of layers: 3
- Activation functions: relu and sigmoid
- Accuracy: 0.7268
- Loss: 0.5527

Second neural network model:
- Number of neurons: 350
- Number of layers: 5
- Activation functions: Sigmoid
- Accuracy: 0.7271
- Loss: 0.5508

Third neural network model:
- Number of neurons: 1125
- Number of layers: 5
- Activation functions: relu and sigmoid
- Accuracy: 0.7280
- Loss: 0.5517

Fourth neural network model:
- Number of neurons: 350
- Number of layers: 5
- Activation functions: tanh, relu, sigmoid
- Accuracy: 0.7230
- Loss: 0.5534

I was not able to achieve the target model performance.
The steps that I took to try to increase model performance is adding more hidden layers, increase the neurons, changing the activation function, increasing epochs, and dropping more columns.


## Summary: 
Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.

