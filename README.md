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
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT
- IS_SUCCESSFUL

Variable are neight targets nor features
- EIN
- NAME
- STATUS

### Compiling, Training, and Evaluating the Model
Initial neural network model:

![Original_Model](https://user-images.githubusercontent.com/110945895/213062510-15aaf3eb-0cf0-4b41-9a48-bf340f0f7eb0.png)

Figure 1. The layers of the original neural network model. 
Removed status
- Number of neurons: 110
- Number of layers: 3
- Activation functions: relu and sigmoid
- Accuracy: 0.7268
- Loss: 0.5527

![Second_Model](https://user-images.githubusercontent.com/110945895/213062565-a60f43bd-3deb-465d-9c92-4779e290c4e6.png)

Figure 2. The layers of the second neural network model. 
Second neural network model:
- Number of neurons: 350
- Number of layers: 5
- Activation functions: Sigmoid
- Accuracy: 0.7271
- Loss: 0.5508

![Third_Model](https://user-images.githubusercontent.com/110945895/213062577-d4cf0360-d382-4151-9653-cd81a65541d3.png)

Figure 3. The layers of the third neural network model.
Third neural network model:
- Number of neurons: 1125
- Number of layers: 5
- Activation functions: relu and sigmoid
- Accuracy: 0.7280
- Loss: 0.5517

![Screen Shot 2023-01-17 at 7 59 39 PM](https://user-images.githubusercontent.com/110945895/213062597-7bd39bd2-6fa5-4899-8218-90247d9c39a6.png)

Figure 4. The layers of the forth neural network model.
Fourth neural network model:
- Number of neurons: 401
- Number of layers: 5
- Activation functions: tanh, relu, sigmoid
- Accuracy: 0.7230
- Loss: 0.5534

I was not able to achieve the target model performance.
The steps that I took to try to increase model performance is adding more hidden layers, increase the neurons, changing the activation function, increasing epochs, and dropping more columns. When I was creating more models, I noticed that the model stop learning after about 20 epochs.


## Summary: 
The goal for this project was to employ machine learning to predict effective funding targets based on historical data. For this task, we employed a fully connected network with four design variations. 

Out of the four models, the third achieved the highest accuracy score of 72.80% and featured the highest neuron count of 1125 neurons. The activation function for the hidden layers were relu while the output layer used the sigmoid activation function. The sigmoid function was employed to display the output as being between 0 (failure case) and 1 (success case). This neural network model was trained for 25 epochs, however, the accuracy plateaued after about 5 epochs. 

A different model could be used to solve this classification problem. I would recommend using a logistic regression model due to its ability of determining a probability of a variable belonging to one of two groups. Since we are trying to determine whether the funding was successful or not, this would be ideal use case for logistic regression. 



