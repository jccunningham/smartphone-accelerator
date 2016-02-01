---
title: "README.md"
author: "J Cunningham"
date: "31 January 2016"
output: html_document
---


The run_analysis.R file in this repo processes data from the 'Human Activity Recognition Using Smartphones Dataset Version 1.0'
prepared by the Smartlab - Non Linear Complex Systems Laboratory in Genoa, Italy (www.smartlab.ws). 

##SOURCE DATA
This dataset is provided in the getdata-projectfiles-UCI HAR Dataset.zip file in this repo.  It can also be retrieved from  https://d396qusza40orc.cloudfront.net/getdata%2Fprojectfiles%2FUCI%20HAR%20Dataset.zip. Please refer to the README.txt file inside the zip folder for the data owners' conditions of use.

The source dataset contains accelerometer measurements taken from a Samsung Galaxy S smartphone while the wearer 
undertook six physical activities. Data for 30 subjects is available. Some data are mean and standard deviation calculations of other observations. Data is split between training and test sets

##PROCESSING
The run_analysis.R file extracts and presents the mean and stdev data in two tidy datasets:
    meansandstdevs -- a processed extract of mean and standard deviation observations
    groupedmeansandstdevs --the mean values of the data in the meansandstdevs dataset, grouped by subject and activity
    
This data processing is an assignment in John Hopkins University's "Getting & Cleaning Data" MOOC offerend on Coursera. Information about processing steps and descriptions of the data variables are given in the Codebook.md file.

Required setup for run_analysis.R:
* extract the contents of the zip file to a folder called UCI HAR Dataset in your R working directory
* install the dplyr package

##KEY FILES

*run_analysis.R -- data processing file

*Codebook.md - a description of source data, processing steps and output files

*meansandstdevs.csv  -- a tidied dataset derived from the source data, an output of run_analysis.R

*groupedmeansandstdevs.csv  -- a tidied dataset derived from the source data, an output of run_analysis.R

*groupedmeansandstdevs.txt  -- a text version of above file

*getdata-projectfiles-UCI HAR Dataset.zip -- the unprocessed source data


###KEY FILES IN SOURCE DATA ZIP FILE

* README.txt - data owner's summary and conditions of use
* Human+Activity+Recognition+Using+Smartphones.htm -- data owners' codebook
* X_train.txt - accelerometer measurements from the training set
* X_test.txt - accelerometer measurements from the training set
* y_train.txt - activity label data corresponding to  x_train.txt measurements
* y_test.txt - activity label data corresponding to  x_test.txt measurements
* subject_train.txt  -subject label data corresponding to  x_train.txt measurements 
* subject_test.txt  -subject label data corresponding to  x_test.txt measurements 
* features.txt - descriptions of the measurements in x_train.txt and x_test.txt
* activity_labels.txt - descriptions of the activities in y_train.txt and y_test.txt

