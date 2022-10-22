# Neural_Network_Charity_Analysis

# Overview of the analysis: Explain the purpose of this analysis.

The purpose of this analysis is to help Beks' foundation to predeict where to make investments. Based on the knowledge of machine learning and neural networks, we will use the features in the provided dataset (charity_data.csv) to help create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. For this analysis we are doing the following: 

      1: Preprocessing Data for a Neural Network Model
      2: Compile, Train, and Evaluate the Model
      3: Optimize the Model


# Results: 
  # Data Preprocessing

* What variable(s) are considered the target(s) for your model?
     
     - Based on the data the target variables are the APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT and IS_SUCCESSFUL columns.

* What variable(s) are considered to be the features for your model?
     
     - Based on the data the target variable is the "IS_SUCCESSFUL" column.
      
* What variable(s) are neither targets nor features, and should be removed from the input data?
     
     - The variables that are neither targets nor featues are the EIN and NAME columns, these were removed. These variable will not increase the accuracy of the model. 
      

# Compiling, Training, and Evaluating the Model

* How many neurons, layers, and activation functions did you select for your neural network model, and why?

     - In the model below, we can see that layer 1 started with 100 neurons with a relu activation. For layer 2, it dropped to 50 neurons and continued with the relu activation. For the final layer, layer 3, it started with 20 neaurons, this seemed to be the better and more accurate. 
     
     ![Pictures/pic%201](https://github.com/cbrito3/Neural_Network_Charity_Analysis/blob/main/Pictures/pic%201.png)
     
  
* Were you able to achieve the target model performance?
      
     - No, the original target for the model was 75%; however, the model for this is under 75%. 


* What steps did you take to try and increase model performance?

     - The steps that were taken to increase model performance were to drop two variables: STATUS and SPECIAL_CONSIDERATIONS.However, these changes did not affect too much the accuracy. 
     
      ![Pictures/pic%202](https://github.com/cbrito3/Neural_Network_Charity_Analysis/blob/main/Pictures/Pic%202.png)
     
     
      ![Pictures/pic%203](https://github.com/cbrito3/Neural_Network_Charity_Analysis/blob/main/Pictures/Pic%203.png)

# Summary: 

 After attempts to modify the data to target the model performance of 75% and using relu and sigmoid activtions, the accuracy was under 75%. One thing to consider next time would be to consider activating functions such as adding more layers and/or dropping other variables. 
      
