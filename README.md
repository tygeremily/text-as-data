# text-as-data
Use supervised learning techniques to classify data in the form of text.

## Introduction
The first part of this file is a simple example of using supervised learning to classify a new observation from previously labeled data in the emaildata.csv. This example is done twice, with and without smoothing. 

Next, the yelp_copy.csv contains data with the following features: business_id, date, review_id, stars, text, type, user_id, cool, useful, funny.  After subsetting the data into training and test sets, the gitDictionary.csv is used to classify the preprocessed words in the review as positive or negative; the dictionary can be found on GitHub by Hu Liu 2004).  A linear support vector machine (SVM) model is used to predict if the reviews are positive or negative.  The results are plotted with a histogram and I use the confusion matrix to compute the accuracy, precision, reall, and F1 score of the sentiment classifier.  The SVM model is then repeated twice, with smooth = 1, prior = "docfreq" and smooth = 0, prior = "uniform". 

Last, I use randomForest to find the variable importance and plot the results. 

## Technologies 
* R Version 4.0

## Libraries/Packages 
* caret
* quanteda
* dplyr
* randomForest
* ggplot2

## File Information
* Data: emaildata.csv, gitDictionary.csv, yelp_copy.csv
* Code: text-data.rmd
