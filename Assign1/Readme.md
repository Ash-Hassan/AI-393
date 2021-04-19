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
After that we normalize the pixels(data) and split x and y for training and testing.
Further we train the regression model and check the accuracy and it was too low to be used.
Then we train naive bayes models and check the accuracy it was good but not the best.
lastly we train the SVM model and saw that it had the best accuracy among all which was 0.97 but for svm model to perform better all i needed to do was apply grid search and tune the parameters so i got the accuracy of 98%.
Finally we used the SVM model to do the prediction and got the score of 0.98 on kaggle.

## Problems Faces ##

### Problem 1:Low knowledge of Data Science. ###
Currently doing a course from Frontier Technolodgy Institue which helped.

### Problem 2: When using regression Got really low accuracy. ###
regression was not working great so i changed the model from reggression to naive bayes then to svm.

### Problem 3: Exporting the file was not in correct format as indexing was also in the file with 'ImageId' and 'Label'. ###
Turns out we only needed was to add a parameter of index=False when using to_csv() function.

### Problem 4: Time Constarint as this semester there was a lot of quizes and assignments ###
working late at night :)

## References ##
- Basic syntax of svm: https://scikit-learn.org/stable/modules/svm.html#classification
- Many other website for sytax checking and eleminating errors.
