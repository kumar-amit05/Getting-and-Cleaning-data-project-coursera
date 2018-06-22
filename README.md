# Getting-and-Cleaning-data-project-coursera
This is the course project for Getting and Cleaning Data course on Coursera. Code is written in R in file. Source file is run_analysis.R. This R script does the following things:
1. Load Packages and get the Data
2. List all the files of UCI HAR Dataset folder The files that will be used to load data are listed as follows: test/subject_test.txt test/X_test.txt test/y_test.txt train/subject_train.txt train/X_train.txt train/y_train.txt
3. Load activity, subject and feature info. Read data from the files into the variables.
4. Merges the training and the test sets to create one data set.
5. Extracts only the measurements on the mean and standard deviation for each measurement. Subset Name of Features by measurements on the mean and standard deviation. Subset the data frame Data by selected names of Features.
6. Uses descriptive activity names to name the activities in the data set.
7. Appropriately labels the data set with descriptive variable names.
8. Creates a independent tidy dataset that consists of the average (mean) value of each variable for each subject and activity pair.
