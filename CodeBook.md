# Code book for Coursera *Getting and Cleaning Data* course project

### Description
Additional information about the variables, data and transformations used in the course project for the Johns Hopkins Getting and Cleaning Data course.

### Overview
30 volunteers performed 6 different activities while wearing a smartphone. The smartphone captured various data about their movements.

### Files
features.txt: Names of the 561 features.
activity_labels.txt: Names and IDs for each of the 6 activities.
X_train.txt: 7352 observations of the 561 features, for 21 of the 30 volunteers.
subject_train.txt: A vector of 7352 integers, denoting the ID of the volunteer related to each of the observations in X_train.txt.
y_train.txt: A vector of 7352 integers, denoting the ID of the activity related to each of the observations in X_train.txt.
X_test.txt: 2947 observations of the 561 features, for 9 of the 30 volunteers.
subject_test.txt: A vector of 2947 integers, denoting the ID of the volunteer related to each of the observations in X_test.txt.
y_test.txt: A vector of 2947 integers, denoting the ID of the activity related to each of the observations in X_test.txt.

### Variables
1. X_train, y_train, X_test, y_test, subject_train and subject_test contain the data from the downloaded files.
2. x_all, y_all and subject_all merge the previous datasets to further analysis.
3. features contains the correct names for the x_all dataset, which are applied to the column names stored in features_mean_std, a numeric vector used to extract the desired data.
4. A similar approach is taken with activity names through the activity_labels variable.
5. x_extract contains a table with the features selected
6. all_data merges x_all, y_all and subject_all in a big dataset.
7. Finally, tidy contains the relevant averages which will be later stored in a .txt file. ddply() from the plyr package is used to apply numcolwise() and ease the development.
