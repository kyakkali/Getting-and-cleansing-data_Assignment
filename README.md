---
title: "README"
author: "Kalpana"
date: "April 21, 2016"
output: html_document
---
### README - Tidy Data Project **
 
This document explains on  how to create tidy data set from many raw data files. 

### Original data source background 
The data in the "Human Activity Recognition Using Smartphones Dataset Version 1.0"   have been taken from experiments carried out with a group of 30 volunteers within an  age bracket of 19-48 years. Each person performed six activities (WALKING, WALKING_UPSTAIRS, WALKING_DOWNSTAIRS, SITTING, STANDING, LAYING) wearing a smartphone (Samsung Galaxy S II) on the waist. Using its embedded accelerometer and gyroscope, 3-axial linear acceleration and 3-axial angular velocity at a constant rate of 50Hz data were captured. The experiments were video-recorded to label the data manually. The obtained dataset was randomly partitioned into two sets, where 70% of the volunteers was selected for generating the training data and 30% the test data.


### The original dataset included the following data files:
     
      *'features.txt': List of all features.
    
      *'activity_labels.txt': List of class labels and their activity name.
    
      *'train/X_train.txt': Training set.
    
      *'train/y_train.txt': Training labels.
    
      *'train/subject_train.txt': ID's of subjects in the training data
    
      *'test/X_test.txt': Test set.

      *'test/y_test.txt': Test labels.

      *'test/subject_test.txt': ID's of subjects in the training data


###  A brief description of the script:
 
Run_Analysis.R R-script on Human Activity Recognition Using Smartphones Dataset

The run_analysis.R script reads data from the "Human Activity Recognition Using        Smartphones Dataset Version 1.0" and produces a new - tidy - dataset which may be used for further analysis.

1. First setting up the working directory. Load reference tables
2. Reading data into table from the  train text files
3. Assign column headings
4. Compiling to  one train data set 
5. Putting together test data
6. Reading data into table from the  train text files
7. Assign column headings
8. Compiling to  one test  data set 
9. Combining train and test data sets to totaldataset
10. Finding the mean and std columns 
11. Assigining descriptive activity labels for activity 
12. Summarizing  tidydata set by subject and Activity
13. Removing "-,()"from the columnnames
14. Creating  Independent data set  with averages of each activity 
15. Create a file with the new tidy dataset
 
 
                  ***********************************************
 
