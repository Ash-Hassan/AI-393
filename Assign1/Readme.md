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
We got the dataset from kaggle both Test and Train data and then submit the predicted data there and got the score/accuracy of 0.97.

## Approach ##
First we loaded the data and check the data for any errors or null basicaly perform the Exploratory Data Analysis.
After that we did the a/b testing using chi-Square and reduced the feature/columns to 587 from 784.
Then we splited the data 80% for training  and 20% for testing with some random states.
Further we train the model with the training data with 587 features as X and the 'label' with Y.
Moreover we tested the model by doing the prediction with 20% data that was splitted earlier.
Lastly we checked the accuracy of the models and did the prediction of the real test data from kaggle.
Finally we submitted the prediction in the right format on the kaggle and got the score of 0.97.

## Problems Faces ##

### Problem 1:Low knowledge of Data Science. ###
Currently doing a course from Frontier Technolodgy Institue which helped.-->

### Problem 2: When using regression Got really low accuracy/when using all features. ###
regression was not working great and i needed to reduce the features as well so i used chi square for that and changed the model from reggression to svm.

### Problem 3: Exporting the file was not in correct format as indexing was also in the file with 'ImageId' and 'Label'. ###
Turns out we only needed was to add a parameter of index=False when using to_csv() function.

### Problem 4: Time Constarint as i started the project three days before deadline ###
working late at night :)

## References ##
- Basic syntax of svm: https://scikit-learn.org/stable/modules/svm.html#classification
- Many other website for sytax checking and eleminating errors.-->
