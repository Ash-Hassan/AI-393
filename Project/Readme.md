# AI 106393: An AI course project #
### PROJECT MEMBERS ###
StdID | Name
------------ | -------------
**64156** | **Hassan Zaheer** <!--this is the group leader in bold.-->
64251 | Areeba Behzad
63650 | Dua Javeria
<!-- Replace name and student ids with acutally group member names and ids-->

## Description ##
This repository contains the Final Project submitted to AI course offered in Spring 2021 at PafKiet.
We got the dataset from kaggle both Test and Train data and then apply convolution after which we train the models and selected the best Combo which was svm and 5x5inc.Then we submited the predicted data on kaggle and got the score/accuracy of 0.98.

## Approach ##

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

#### Approach 3: Deceptively Complex ####
- Following the lead of approach 2 here we will also reduce the features but with a twist.
- We will be using convolution filter technique to reduce the features and only use those features that are related to the target column.
- Then check the outputed datasets with diffrent clasification models.
- Select the most accurate one and make the predictions!!

#### Approach 4: Going all Out ####
- Use Deep learning models like CNN and make predictions on it i saw on kaggle people have acchived 100% with it.
- It requires extensive research, computation power and domain knowledge.

### Approach I Implemented was Deceptively Complex ###
- First the data is loaded and checked for any errors or null basicaly perform the Exploratory Data Analysis.
- After that I splited x and y for the convolution.
- Here we use 3 sizes 5x5,7x7 and 9x9 with 2 different filters.
- By doing this I got 6 unique datasets with reduced features.
- Then we apply 4 ML models(LR,KNN,SVM,NB) on those 6 datasets.
- After that we saw the best combo that has the highes accuracy was the 5x5(wighted filter) and SVM(hyperTuned) model.
- It had the best accuracy among all which was 98.08%.
- Then I imported the testing dataset and apply the same convolution on it to match the number of features.
- Finally we used that combo model to do the prediction and got the score of 0.9808 on kaggle.

## Problems Faces ##

### Problem 1:Very little info available about the convolution filters. ###
- When we write convolution filters on the internet the only thing pops up is the CNN model as that uses convolution with kernal size. After extensive resarch i found the scipy libray that basically makes the layers of CNN and do the convolution part. Thats how i was able to use the covolution.

### Problem 2:Reduced Features. ###
- After applying Convolution on training dataset the number of features got reduced which is good but the same number of features was on test dataset to make the predictions and it's very time consuming to run convolution again and again even on kaggle.

### Problem 3: Very high computational cost. ###
- As i was running convolution almost 7 times and i was applying 4 ML models on each and every data set so almost 24 models were implemented and that alone took too much computation. My notebook on kaggale almost took 2.30 hours just execute all cells to save the error less file.

### Problem 4:Low knowledge of Data Science. ###
- Currently doing a course from Frontier Technolodgy Institue which helped.

### Problem 5: Exporting the file was not in correct format as indexing was also in the file with 'ImageId' and 'Label'. ###
- Turns out we only needed was to add a parameter of index=False when using to_csv() function.

### Problem 6: Time Constarint as this semester there was a lot of quizes and assignments ###
- Working late at night :)

## References ##

- Basic syntax of Each Prediction model : https://scikit-learn.org/
- Convolution Filter : https://docs.scipy.org/doc/scipy/reference/generated/scipy.signal.convolve2d.html#scipy.signal.convolve2d
- Many other website for sytax checking and eleminating errors.
