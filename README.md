# Neural_Network_Charity_Analysis

## Overview of the analysis: 
The purpose of this analysis is to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results: 

### Data Preprocessing

![image](https://user-images.githubusercontent.com/85706721/141663500-215429f3-56fa-48ce-b632-cdaae81a8a86.png)

- What variable(s) are considered the target(s) for your model?
  - My target variable is "IS_SUCCESSFUL".

- What variable(s) are considered to be the features for your model?
  - In my model I considered the following variables as features:
    - STATUS 	
    - ASK_AMT 	
    - APPLICATION_TYPE_Other 	
    - APPLICATION_TYPE_T10 	
    - APPLICATION_TYPE_T19 	
    - APPLICATION_TYPE_T3 	
    - APPLICATION_TYPE_T4 	
    - APPLICATION_TYPE_T5 	
    - APPLICATION_TYPE_T6 	
    - ... 	
    - INCOME_AMT_1-9999 	
    - INCOME_AMT_10000-24999 	
    - INCOME_AMT_100000-499999 	
    - INCOME_AMT_10M-50M 	
    - INCOME_AMT_1M-5M 	
    - INCOME_AMT_25000-99999 	
    - INCOME_AMT_50M+ 	
    - INCOME_AMT_5M-10M

- What variable(s) are neither targets nor features, and should be removed from the input data?
  - EIN
  - NAME

  ![image](https://user-images.githubusercontent.com/85706721/141663595-13ac9001-032e-4762-aa21-c0d05a482309.png)


### Compiling, Training, and Evaluating the Model
- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - I opted to go with 3 layers and I chose 150 neurons for my first layer, 100 for my second layer, and 50 for my third layer.  I decided to stick with 3 layers because this was already a long running process and adding a 4th seemed too much.  I chose my number of neurons after trying various other values, some lower than the original amount but those resulted in much lower accuracy.
 
      ![image](https://user-images.githubusercontent.com/85706721/141663413-9f9e6969-3602-4db7-8af0-201c20efc042.png)

- Were you able to achieve the target model performance?
  - No, I was not.   
 
- What steps did you take to try and increase model performance?
  - I tried several combinations of activation functions and most resulted in much lower accuracy.  I also played around with the number of neurons and layers. Most of these changes resulted in lower accuracy and others came close, but did not improve over the original combination.

## Summary: 

This deep learning model ended up with a 73% accuracy.  This is a good starting point, but it could be better. I would continue fine tuning this model, but try more layers and more neurons.
