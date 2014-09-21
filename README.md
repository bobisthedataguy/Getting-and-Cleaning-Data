###Getting-and-Cleaning-Data

### Introduction
 
This reponsitory contains deliverables submitted in fullfillment of the Johns Hopkins "Getting and Cleaning Data" course project requirement. This course was presented via Coursera. The purpose of this project is to demonstrate the ability to collect, work with, and clean a data set. The goal is to prepare a "tidy" data that can be used for further analysis. Project requirements are included in the "project_requirements.txt" file contained within this repo. The following is required for submission:

1) a tidy data set

2) a link to this Github repository containing the script

3) a code book 

Smart phone data collected from subjects while performing six activites was collected through a prior independant study^1. This data has been made available for use educational purposes. More details on this data can be found in the Codebook. The script in this repo reformats this data in order to make it more usable for later analysis.

### How does it work?

The script "run_analysis.R" contained within this repo is used to create the 'tidy' dataset. This script takes the "Human Activity Recognition Using Smartphones Dataset" as input. The following processing is performed within this script:

- Installs required packages if not already installed
- loads features (measure column headings) data and determines which columns are Mean and Standard Deviation measures
- loads the activty labels data. This will allow the activity names (e.g. WALKING, STANDING, etc.) to be looked up based upon the activity code contained in the main dataset
- loads and assembles the training dataset, combining the subject values, activity names, and only the mean and standard deviation measures
- loads and assembles the testing dataset, combining the subject values, activity names, and only the mean and standard deviation measures
- combines the training dataset and the testing dataset
- computes averages (mean) of each measure value for each subject/activity combination
- outputs the resulting data to the "tidy" data file

### Required Packages

reshape2

### Resulting data set

The resulting "tidy" dataset can be found in the "tidy_data.txt" file. The link is below:

https://github.com/bobisthedataguy/Getting-and-Cleaning-Data/blob/master/tidy_data.txt

### Codebook

The Codebook is available in the CODEBOOK.md file contained within this Repo. The link is below:

https://github.com/bobisthedataguy/Getting-and-Cleaning-Data/blob/master/CODEBOOK.md


### References

[1] Davide Anguita, Alessandro Ghio, Luca Oneto, Xavier Parra and Jorge L. Reyes-Ortiz. Human Activity Recognition on Smartphones using a Multiclass Hardware-Friendly Support Vector Machine. International Workshop of Ambient Assisted Living (IWAAL 2012). Vitoria-Gasteiz, Spain. Dec 2012
