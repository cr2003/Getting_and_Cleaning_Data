Getting_and_Cleaning_Data
=========================

Coursera Getting and Cleaning Data Project

This repo contains the R scripts that can be used to analysis the [UCI HAR Dataset](http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones) and convert it into a tidy data set.

This was done as the course project for the "Getting and Cleaning Data" course in Coursera which is part of the "Data Science" specialization

## Requirements

Create a R script that does the following

* Merges the training and the test sets to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set
* Appropriately labels the data set with descriptive variable names.
*From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject.

## How to run the R script code

The R code that is used for analysis is available in the [run_analysis.R](run_analysis.R) file, the script does the following:

* Bind the training and the test serts to create one data set.
* Extracts only the measurements on the mean and standard deviation for each measurement.
* Uses descriptive activity names to name the activities in the data set (columns name)
* Appropriately labels the data set with descriptive activity names.
* Creates the final tidy data set with the average of each variable for each activity and each subject.

It is neccessary to have the libraries `dplyr`and `magrittr` installed for running `run_analysis.R`.

## The tidy data

The final tidy data set it is created in the working directory and can be loaded back into an R table using the following command
```R
tidydata <- read.table("tidydata.txt")
```
## Data Code Book

The [codebook](CodeBook.md) available in this repo describes the variables, the data, the transformations that are done and the clean up that was performed on the data
