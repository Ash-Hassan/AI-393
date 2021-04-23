# AI 106393: An AI course project #
### PROJECT MEMBERS ###
StdID | Name
------------ | -------------
**64156** | **Hassan Zaheer** <!--this is the group leader in bold.-->
64251 | Areeba Behzad
63650 | Dua Javeria
<!-- Replace name and student ids with acutally group member names and ids-->

## Description ##
This repository contains assignment 1 submitted to AI course offered in Spring 2021 at PafKiet.
We got the dataset from kaggle both Test and Train data and then train the models and selected the best model which was svm.Then we submited the predicted data on kaggle and got the score/accuracy of 0.98.

## Approach ##
==============
### Possible Approaches ###
#### Approach 1: Keeping it Simple ####
- Load the datasets
- Train the models(linear Regression,Svm,NB,etc)
- Evaluate the models based on accuracy
- Find the accurate model and make the predictions
- Output the file and submit on kaggle

#### Approach 2: Simple yet Complex ####
- The only issue with the simple approach is it has large number of features so in this approach we can reduce it.
- Using chi-square, Selectkbest, etc.

#### Approach 3: Going all Out ####
- Use Deep learning models like CNN and make predictions on it i saw on kaggle people have acchived 100% with it.
- It requires extensive research, computation power and domain knowledge.

### Approach I Implemented ###
- First the data is loaded and checked for any errors or null basicaly perform the Exploratory Data Analysis.
- After that we normalize the pixels(data) and split x and y for training and testing.
- Further we train the regression model and check the accuracy and it was too low to be used.
- Then we train naive bayes models and check the accuracy it was good but not the best.
- lastly we train the SVM model and saw that it had the best accuracy among all which was 0.97 but for svm model to perform better all i needed to do was apply grid search and tune the parameters so i got the accuracy of 98%.
- Finally we used the SVM model to do the prediction and got the score of 0.98 on kaggle.
- I have not uploaded the code of Gridsearch and chisquare but i have implemented both seprately and got the required parameters for svm where as the chisquare as more or less performing the same as taking all the features so i dropped the idea of chisquare.

## Problems Faces ##
====================

### Problem 1:Large Number of Features for training. ###
- In training data we have 784 Features which quite large for training, So we have to reduce the columns by using some technique's like chisquare,Convolution filters etc. But the problem with chi-square is that it is used between to catagorical variables and for convolution filter it was applied in final project.

### Problem 2:Normalizing the Features. ###
- In training data we have to normalize the features in order to bring balence among every feature and same goes for the Testing data! i forgot to do it on testing data and struggled to find the solution as the model was lagging and getting hanged, But after normalization on testing everything runs smooth.

### Problem 3:Low knowledge of Data Science. ###
- Currently doing a course from Frontier Technolodgy Institue which helped.

### Problem 4: When using regression Got really low accuracy. ###
- Regression was not working great so i changed the model from reggression to naive bayes then to svm.

### Problem 5: Exporting the file was not in correct format as indexing was also in the file with 'ImageId' and 'Label'. ###
- Turns out we only needed was to add a parameter of index=False when using to_csv() function.

### Problem 6: Time Constarint as this semester there was a lot of quizes and assignments ###
- Working late at night :)

## References ##
================
- Basic syntax of Each Prediction model : https://scikit-learn.org/
- Many other website for sytax checking and eleminating errors.
