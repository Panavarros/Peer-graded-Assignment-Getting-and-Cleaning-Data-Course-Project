Human Activity Recognition Using Smartphones Dataset" Getting and Cleaning Data - Course Project.

This repository is a Paula Navarro submission for Getting and Cleaning Data course project.The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare tidy data that can be used for later analysis. The script was developed to analyze some descriptive statistical measures, from the data from UCI HAR Dataset. 

The original files come from Machine Learning Repository. The data correspond to "Human Activity Recognition database" built from the recordings of 30 subjects performing activities of daily living (ADL) while carrying a waist-mounted smartphone with embedded inertial sensors. Available here https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip

The following files from the initial dataset is used:

1. features.txt - includes the descriptions for features measured
2. train/X_train.txt - includes the measurements of the features in train set (one row - 1 measurement of 561 features)
3. test/X_test.txt - includes the measurements of the features in test set
4. train/subject_train.txt - subject for each measurement from the train set
5. test/subject_test.txt - subject for each measurement from the test set
6. train/y_train.txt - activity (from 1 to 6) for each measurement from the train set
7. test/y_test.txt - activity (from 1 to 6) for each measurement from the test set

In the present repository "Peer-graded-Assignment-Getting-and-Cleaning-Data-Course-Project" three files are present:

- CodeBook.md
- Readme.md
- run_analysis.R

-CodeBook.md describes the data sets and variables in a more detail was.
-run_analysis.R is an R script that is doing following:
1) Download the dataset from web if it does not already exist in the working directory.
2) unzip the files from a zip file and get the list of it.
3)Read train data sets and explore some properties of the previous variables.: Activity files ("Y_test.txt", "Y_train.txt"), Subject files ("subject_train.txt", "subject_test.txt") and Fearures files ("X_test.txt", "X_train.txt").
4) Merges the training and the test sets to create one data set. Concatenate the data tables by rows (dataSubject, dataActivity, dataFeatures)
5) It Extracts the measurements on the mean and standard deviation for each measurement.
6) Change the names of the activities in the data set for descriptive activity names.
7) Change the state labels the data set to descriptive variable names.
8) Creates final tidy data set and output it.
9) Create a codebook
