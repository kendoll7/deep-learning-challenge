# deep-learning-challenge
module-21-challenge

used instructor videos and notes from class to complete this assignment

*#The report should contain the following:

#Overview of the analysis: Explain the purpose of this analysis.

#Results: Using bulleted lists and images to support your answers, address the following questions:

#Data Preprocessing

1. What variable(s) are the target(s) for your model?

The target is the Is_Successful column.

2. What variable(s) are the features for your model?

The features of this model are the APPLICATION_TYPE,	AFFILIATION,	CLASSIFICATION,	USE_CASE,	ORGANIZATION,	STATUS,	INCOME_AMT,	SPECIAL_CONSIDERATIONS,	ASK_AMT	IS_SUCCESSFUL

3. What variable(s) should be removed from the input data because they are neither targets nor features?

The EIN number was dropped.

#Compiling, Training, and Evaluating the Model
1. How many neurons, layers, and activation functions did you select for your neural network model, and why?

For this model, 3 hidden layers each with many neurons were used. This was used because the compute seems to increase the accuracy above 75%. The first activation is relu and the second and third activations are sigmmoid. The hope is to boost accuracy of my model. The names column was added back to get better scores.

2. Were you able to achieve the target model performance?

Yes.

3. What steps did you take in your attempts to increase model performance?

The NAME column was kept and converted into data points to improve the model's performance. This had the biggest impact, but required another layer with sigmoid activation which is costly.

##Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation*

Overall the accuracy was above the 75% threshold and we are able to correctly classify each applicant in the test 75% of the time.

An applicant has an 80% chance of being successful if they fall into these parameters:

Name of applicant appears more than 5 times
Type of application is in T3, T4, T5, T6, T7, T8, T10, or T19 
The classification of the applicant is C1000, C2000, C1200, C2100, or C3000     

I recommend the RandomForest model as it reduces the effect of outliers and is also fairly accurate with a score over 75%
