Getting and Cleaning Data Course Project
========================================
This file describes how run_analysis.R script works.
* First, unzip the data from https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip 
* Set the working directory where you are extracting this zip file for example: setwd("C:\\Users\\mbhadaur\\Downloads\\UCI HAR Dataset\\UCI HAR Dataset").
* Make sure the run_analysis.R script is present in the current working directory.
* Second, open this run_analysis.R" file in R editor and run it from the editor. 
* Third, you will find two output files are generated in the current working directory:
  - merged_data.txt (8083 Kb): it contains a data frame called finaldata with 10299*68 dimension.
  - data_with_means.txt (217 Kb): it contains a data frame called finalresult with 180*68 dimension.
* Finally, use data <- read.table("data_with_means.txt") command in R console to read the file. Since we are required to get the average of each variable for each activity and each subject, and there are 6 activities in total and 30 subjects in total, we have 180 rows with all combinations for each of the 66 features. 
