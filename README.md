# Getting-anCleaning-Data-Week-4-Assignment
Repository fot the assignment of Getting and Cleaning Data course.

Instructions:  download and unzip the data file into your R working directory.
then, download the R source code into your R working directory.
Finally, execute R source code to generate tidy data file.
 ## Description of Data
The Data X variables are sensor signals measured from 30 subjects with waist-mounted smartphones.The Data Y variable indicates the type of operation the subjects performed during the recording.
### explaination of code
The code merged training dataset and test dataset, and extracted partial variables to create a separate dataset with the averages for each operation.
 ## dataset
The new produced data set included estimated mean and standard deviation variables.For all subjects, every dataset row is an average of any form of operation.

## The code was drawn up based on the instruction sted in cousera week 4 assignment

In R setting, read training and test data collection.
Write names of variable in envrionment of R.
Read the index of topic into R environment.
##
A Combines the training and the test sets to produce one set of data. 
Using rbind command to combine exercise and test package
B Collects for each calculation only the results on mean and standard deviation. Using the grep command to get variable name column indexes containing "mean)" (or "std)"
C Used descriptive activity names to name the task in the data set Convert task labels to characters and add a new column as factor
D The data set is correctly labelled with the descriptive names of the element.Give variable columns with the selected descriptive names.
E From the data set in step D, generates a second, separate set of tidy data for each operation and topic with the average of each variable.Using pipeline to build a new tidy dataset with group by command and summarize each in dplyr package
