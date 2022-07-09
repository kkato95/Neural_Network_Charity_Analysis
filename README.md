# Neural_Network_Charity_Analysis

## Overview of Analysis - Purpose of Analysis

The purpose of this analysis is to use machine learning and nerual networks to predict where to make investments. We are creating a binary classifier that predicts the whether or not the application will be susccessful if funded by AlphabetSoup. The dataset contains information on the organizions funded by AlphabetSoup.


Deliverable 1: 
The analysis included binning the values in several of our columns, then merged the OneHotCoded features into single dataframe. Next, we scaled the data.

Deliverable 2:
The purpose of this deliverable is to run the deep neural network. We bgan by declaring a sequantial nerual model, then we added the hidden layers. Then the model was complied and train. The evaluation of the model shows an accuracy of .


## Results

#### Data Preprocessing

1. What variables are considered the targets for you model?
The target for our model is the IS_SUCCESSFUL column determining if the funding was paid out on not.

2. What variables are considered to be the features for your model?
The features for our model includes the values for the application_type

3. What variables are neither targets nor features, and should be removed from the input data?
From our initial dataframe, we dropped the EIN and NAME coulmns because it was additional noise that did not add any value. In our optimized file, we determined to drop SPECIAL_CONSIDERATIONS as it provided no value.


#### Compiling, Training, and Evaluating the Model

1. How many neurons, layer, and activation functions did you select from your neural network model, and why?
In our original file we included 3 hidden layers and each layer had 80, 50, and 40 nodes in each layer respectivly. We desired a deep learning neural network due to the complexity of the data. The deep learning neural network will provide highest model accuracy score possible. 

2. Were you able to acheive the target model preformance?
Regarding deliverable 3, where we were to optimize the model, we were not able to reach the desired 75% accuracy score. We were unable to reach a higher accuracy score in our optimized model.


3. What steps did you take to try and increase model preformances?
We tried several things to boost the accuracy score. Our most successful model provided an accuracy score of 72.86% which is .3% greater than the original model. We acheived this by dropping the SPECIAL_CONSIDERATIONS column as well. Then we changed the conditional amount to 800 for classification and 200 for application_type. Lastly, we added 2 more hidden layers with activation 'relu'.


## Summary

The results of our application model are fair. The model predicts correctly 72.86% of the time. We optimized the model by changing minor features of the model. The loss amount is also fairly high, with a value of 0.5523. If we were to create a smiliar model to solve this classification problem, we would acquire more data to run through the model. 
