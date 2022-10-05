# Neural Network Charity Analysis
## Overview and Purpose:




## Results: Using bulleted lists and images to support your answers, address the following questions. 
### Data Preprocessing
#### Target variable 
- The target variable for this dataset is ‘IS_SUCCESSFUL’ and the possible values for this column are 0 or 1.

#### Feature variables
The feature variables in this dataset are:
- APPLICATION_TYPE
- AFFILIATION
- CLASSIFICATION
- USE_CASE
- ORGANIZATION
- STATUS (This variable was removed in the optimization deliverable)
- INCOME_AMT
- SPECIAL_CONSIDERATIONS
- ASK_AMT


#### Variables removed from the dataset during preprocessing.
- Two of the variables, NAME and EIN are not considered to be target or feature variables and were removed during preprocessing 

### Compiling, Training, and Evaluating the Model
#### Neurons, layers, and activation functions.
In the optimization deliverable the neural network consists of three hidden layers and an output layer. 

The first hidden layer contains 80 neurons and the activation function is ‘linear.’
The second hidden layer contains 30 neurons and the activation function is ‘relu.’
The third hidden layer contains 10 neurons and the activation function is ‘relu.’

Lastly, the output layer contains 1 neuron and the activation function is ‘sigmoid.’

#### Did the model reach the target model performance?
Unfortunately I was unable to create a neural network that reached the target performance accuracy. The greatest accuracy I was able to achieve was 0.724.

#### Alterations made to increase model performance.
To increase model performance I binned two columns, ‘INCOME_AMT’ and ‘ASK_AMT.’  
The ‘INCOME_AMT’ column was reduced from 9 unique values to 7. The ‘ASK_AMT’ column was reduced from 8747 unique values to 6.

I removed the variable ‘STATUS’ from the dataset. 

I also altered the amount of neurons, amount of hidden layers, and the activation functions used in the neural network. 
The original neural network in file AlphabetSoupCharity.ipynb only consisted of 2 hidden layers, with 80 and 30 neurons respectively. Both of the hidden layers in the original neural network utilized the activation function ‘relu.’ 
As seen previously in the “Neurons, layers, and activation functions” section, the neural network was altered to contain 3 hidden layers with 80, 30, and 10 neurons respectively. The activation function of the first hidden layer was changed to ‘linear.’   The output layer was not altered from the original neural network. 

## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
