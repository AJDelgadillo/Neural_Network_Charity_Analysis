# Neural Network Charity Analysis
## Overview and Purpose:
The purpose of this challenge was to alter a neural network to increase model performance. In the first two deliverables of this challenge we preprocessed some of the data. We removed two irrelevant variables and binned two other variables. A neural network was created containing two hidden layers and one output layer. 

When completing these two deliverables the model showed an accuracy of 0.725. In deliverables 3 and 4 the goal was to increase the model performance to 0.75. Although I was unable to achieve this goal I have outlined the steps I took in my attempt to increase the performance of the neural network model. 



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

I removed the variable ‘STATUS’ from the dataset. Out of the two possible Values, 0 and 1, 34294 datapoints has a ‘0’ in the ‘STATUS’ column and only 5 datapoints has a ‘1.’ I concluded that since such a large majority of datapoints had the same value, this variable did not introduce a significant variation in data and could be removed without negatively impacting the analysis. 

I also altered the amount of neurons, amount of hidden layers, and the activation functions used in the neural network. 
The original neural network in file AlphabetSoupCharity.ipynb only consisted of 2 hidden layers, with 80 and 30 neurons respectively. Both of the hidden layers in the original neural network utilized the activation function ‘relu.’ 
As seen previously in the “Neurons, layers, and activation functions” section, the neural network was altered to contain 3 hidden layers with 80, 30, and 10 neurons respectively. The activation function of the first hidden layer was changed to ‘linear.’   The output layer was not altered from the original neural network. 

## Summary and Recommendation:

For the optimization deliverable I was unable to achieve the target performance of 0.75. The greatest accuracy I was able to achieve is 0.724. 

Unfortunately I was unable to identify why I was unable to significantly increase the performance of this model. In the future I might suggest that the researcher gather more data, so we have a more diverse dataset to work with. 
When creating the neural network I would continue to try different model structures. It is possible that the model contained too many or too little neurons, or the activation functions used were not compatible with the data being analyzed. Additionally, I would suggest testing different optimizers in the output layer.
