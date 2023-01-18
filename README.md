# Neural_Network_Charity_Analysis
Module 20
## Overview of the analysis: 
With the historical dataset provided by Alphabet Soup including organizations receiving funding over years, it is to create a binary classifier using neural network predicting model capable of predicting whether applicants will be successful if funded by Alphabet Soup.

## Results:

### Data Preprocessing</br>
- What variable(s) are considered the target(s) for your model? </br>
**Ans: The colunm of "IS_SUCCESSFUL" is considered the target of this model.**</br> 
- What variable(s) are considered to be the features for your model?</br>
**Ans: All other columns except "EIN", "NAME" and "IS_SUCCESSFUL" are considered our model features to be independent variables in predicing the target.**</br>
- What variable(s) are neither targets nor features, and should be removed from the input data?</br>
**Ans: "EIN" and "NAME" columns are removed from datafram since they are not considered to be the variables that could imapct the result.**</br>
### Compiling, Training, and Evaluating the Model</br>
- How many neurons, layers, and activation functions did you select for your neural network model, and why?</br>
**Ans: Inital testing model, there are 2 layers with 3 and 5 neurons in each layer as shown below**</br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/initial%20model.png)
- Were you able to achieve the target model performance?</br>
**Ans: Unfortunately, it does not achieve at least 75% or accuracy.**</br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/Initial%20model%20testing%20result.png)
- What steps did you take to try and increase model performance?</br>
**Ans: First step to optimize the model is to identify the best 3 models by defining a new sequential model with three possible choices of activation methodologies, as being shown in the following image**</br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/find%20top%203%20best%20models.png)
**Because the result suggests to activate with "Relu", secondly, I increase gradually the hidden layers and adjust neurons in each attempt, the following snapshots revealing all the 3 attempts with hyperparameters.**</br>
  **1. First Attempt**</br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/1st%20optimization%20attempt.png)</br>
  **2. Second Attempt**</br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/2nd%20optimization%20attempt.png)</br>
  **3. Third Attempt**</br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/3rd%20optimization%20attempt.png)</br>
## Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and explain your recommendation.
Unfortunately, after all three additional attempts, it is found to achive over 74% of accuracy after the 3rd trained model, there is though no model able to achieve 75% of accuracy. It is recommended to still activate with "Relu" due to this activation model is reliable to be trained faster than others. Another thought to improve the model is that it may be benefitial to also increase Epoches when testing the model. The other recommendation is to increase numbers of denses and units to fill the potential gaps, below image is showing a proposed model using Tensorflow playground </br>
![Image](https://github.com/jilldvn/Neural_Network_Charity_Analysis/blob/main/images/NN%20model%20playground.png)
