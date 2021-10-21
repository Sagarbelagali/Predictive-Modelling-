# Predictive-Modelling-
Predictive modelling ML

Answer Report: In this, you need to submit all the answers to all the questions in a sequential manner. It should include the detailed explanation of the approach used, insights, inferences, all outputs of codes like graphs, tables etc. Your report should not be filled with codes. You will be evaluated based on the business report.
Jupyter Notebook file: This is a must and will be used for reference while evaluating.
 

Problem 1: Linear Regression


You are hired by a company named Gem Stones Co Ltd, which is a cubic zirconia manufacturer. You are provided with the dataset containing the prices and other attributes of approximately 27,000 pieces of cubic zirconia (which is an inexpensive synthesized diamond alternative with similar qualities of a diamond).

Your objective is to accurately predict prices of the zircon pieces. Since the company profits at a different rate at different price levels, for revenue management, it is important that prices are predicted as accurately as possible. At the same time, it is important to understand which of the predictors are more important in determining the price.

The data dictionary is given below.

Data Dictionary:

Variable Name

Description

Carat

 Carat weight of the cubic zirconia.

Cut

 Describes the cut quality of the cubic zirconia. Quality is in increasing order: Fair, Good, Very Good, Premium, Ideal.

Colour 

Colour of the cubic zirconia.

Clarity

Cubic zirconia Clarity refers to the absence of the Inclusions and Blemishes. (In order from Best to Worst, FL = flawless, I3= level 3 inclusions) FL, IF, VVS1, VVS2, VS1, VS2, SI1, SI2, I1, I2, I3

Depth

The Height of a cubic zirconia piece, measured from the Culet to the table, divided by its average Girdle Diameter.

Table

The Width of the cubic zirconia's Table expressed as a Percentage of its Average Diameter.

Price

Price of the cubic zirconia.

X

Length of the cubic zirconia in mm.

Y

Width of the cubic zirconia in mm.

Z

Height of the cubic zirconia in mm.


Dataset for Problem 1: cubic_zirconia.csv

 

Following is a guideline for developing a solution

The very first step of any data analysis assignment is to do the exploratory data analysis (EDA). Once you have understood the nature of all the variables, identified the response and the predictors, apply appropriate methods to determine whether there is any duplicate observation or missing data and whether the variables have symmetric or skewed distribution. Note that data may contain various types of attributes and numerical and/or visual data summarization techniques need to be appropriately decided. Both univariate and bivariate analyses and pre-processing of data are important. Check for outliers and comment on removing or keeping them while model building. Since this is a regression problem, the dependence of the response on the predictors needs to be thoroughly investigated.
Use Full Data to develop a model to identify significant predictors. Check whether the proposed model is free of multicollinearity. Apply variable selection method as required. Show all intermediate models leading to the final model. Justify your choice of the final model. Which are the significant predictors?
Alternatively, if prediction accuracy of the price is the only objective, then you may want to divide the data into a training and a test set, chosen randomly, and use the training set to develop a model and test set to validate your model. Use the models developed in Part (2) to compare accuracy in training and test sets. Compare the final model of Part (2) and the proposed one in Part (3). Which model provides the most accurate prediction? If the model found in Part (2) is different from the proposed model in Part (3), give an explanation.
Write a project report on the solution method, clearly highlighting the benefits of both approaches. Your report must indicate the logic of model selection and business interpretation.

 

Problem 2: Logistic Regression and Linear Discriminant Analysis(LDA)


You are hired by a sports analysis agency to understand the selection process of high school football players into college with a full or partial scholarship. You are provided details of 6215 high school graduates who have been inducted into 4-year degree colleges with either full or partial scholarships.  You have to help the agency in predicting whether a high school graduate will win a full scholarship on the basis of the information given in the data set. Also, find out the important factors which are instrumental in winning a full scholarship in colleges.

Dataset for Problem 2: Football Scholarship.csv

Data Dictionary:

Variable Name

Description

Scholarship 

 Won a college scholarship: Full / Partial

Academic Score 

 High school academic performance of a candidate

Score on Plays Made

 A composite score based on the achievements on the field

Missed Play Score

 A composite score based on the failures on the field

Injury Propensity 

 This has 3 ordinal levels: High, Moderate, Normal and Low. It has been calculated based on what proportion of time a candidate had an injury problem

School Type 

 3 types of schools based on their location

School Score 

 A composite score based on the overall achievement of the candidates’ school, based on the schools academic, sports and community service performance

Overall Score

A composite score based on a candidate’s family financial state, school performance, psychosocial attitude etc

Region

Region of the country where the school is located

 

 

Following is a guideline for developing a solution

The very first step of any data analysis assignment is to do the exploratory data analysis (EDA). Once you have understood the nature of all the variables, especially identified the response and the predictors, apply appropriate methods to determine whether there is any duplicate observation or missing data and whether the variables have a symmetric or skewed distribution. Note that data may contain various types of attributes and numerical and/or visual data summarization techniques need to be appropriately decided. Both univariate and bivariate analyses and pre-processing of data are important. Check for outliers and comment on removing or keeping them while model building. For this is a classification problem, the dependence of the response on the predictors needs to be investigated.
Two different classification techniques are to be applied. However, the EDA part remains the same for both.
For easier interpretation of the models, later on, it may be better to code Full = 1 and Partial = 0. You may assume the opposite, but then you have to be very careful about the interpretation of the logistic model coefficients later.

Use Full Data to develop a logistic regression model to identify significant predictors. Check whether the proposed model is free of multicollinearity. Apply variable selection method as required. Show all intermediate models leading to the final model. Justify your choice of the final model. Which are the significant predictors?
Compare values of model selection criteria for proposed models. Compare as many criteria as you feel are suitable.
Alternatively, if prediction accuracy of the full scholarship is the only objective, then you may want to divide the data into a training and a test set, chosen randomly, and use the training set to develop a model and test set to validate your model. Use the models developed in Part (2) to compare accuracy in training and test sets. Compare the final model of Part (2) and the proposed one in Part (3). Which model provides the most accurate prediction? If the model found in Part (2) is different from the proposed model in Part (3), give an explanation.
Use the same training-test data split in Part (3) to develop a suitable linear discriminant model. Use the same to predict discriminant scores for the test data. Compare the final output from the logistic regression model and LDA.
Write a project report on the solution methods, clearly highlighting the benefits of both approaches. Your report must indicate the logic of model selection and business interpretation.
