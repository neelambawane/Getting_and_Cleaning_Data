#Getting and Cleaning Data Course-Project
The run_analysis.R script performs the data preparation and then followed by the 5 steps required as described in the course project's definition.

#Download the dataset 
Downloaded and extracted data under the folder 'UCI HAR Dataset'

#Assign each file to variables
Read the files to variables with names corresponding to the source files

#Step-1: Merges the training and the test sets to create one data set
Test set data were combined together by columns. Train set data were also combined similarly. Test and train set data were combined to create the full data set.

#Step-2: Extracts only the measurements on the mean and standard deviation for each measurement
TidyData is created by subsetting Merged_Data, selecting only columns: subject, code and the measurements on the mean and standard deviation (std) for each measurement.

#Step-3: Uses descriptive activity names to name the activities in the data set
Entire numbers in code column of the TidyData replaced with corresponding activity taken from second column of the activities variable

#Step-4: Appropriately labels the data set with descriptive variable names
Columns in TidyData are renamed into appropriate labels

#Step-5: From the data set in step 4, creates a second, independent tidy data set with the average of each variable for each activity and each subject
FinalData is created by sumarizing TidyData taking the means of each variable for each activity and each subject, after groupped by subject and activity.

Export FinalData into FinalData.txt file.
