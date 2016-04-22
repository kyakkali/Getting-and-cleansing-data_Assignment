---
title: "CodeBook.md"
author: "Kalpana"
date: "April 20, 2016"
output: html_document
---
#### Tidy Data CodeBook
 
   This file describes the variables, the data, and any transformations or work that   have been performed to clean up the data.
#### Sourcing Data

1. The site where the data was obtained:
     http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones
2. The data for the project:
     https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip
     
#### Reading and Loading data from text files

1. The run_analysis.R script performs the following steps to clean the data:
2. Read X_train.txt, y_train.txt and subject_train.txt , feature.txt from the "train" folder    and store them in varibals_train, activity_train and Subject_train variables                 respectively.
3. Read X_test.txt, y_test.txt and subject_test.txt from the "test" folder and store them in     Variables_test, activity_test and subject_test variables respectively.
4. Read the features.txt file from the "UCI HAR Dataset" folder and store the data in a          variable called features.
5. Assign Column headings to subject, activity , train and test variables.

#### Concatenating  train and test data

1. Combine subject, activity , train variables to train data set and subject, acvity and test    variables to test data set using cbind.
2. Concatenate testData to trainData to generate a 10299x563 data frame called totaldataset. 
3. We only extract the measurements on the mean and standard deviation, subject and activity    to tidydata. This results in a 68 indices list. We get a subset of tidydataset with the 68    corresponding columns.

#### Cleansing data & created the tidy data set

1. Assigining descriptive activity labels for each activity. 
2. Clean the column names of the subset. We remove the "()" and "-" symbols in the nameS.
3. Finally, generate a second independent tidy data set with the average of each measurement    for each activity and each subject. We have 30 unique subjects and 6 unique activities,      which result in a 180 combinations of the two. Then, for each combination, we calculate      the mean of each measurement with the corresponding combination. 
4. Write the result out to "tidy_data.txt" file in current working directory.




                   ******************************************