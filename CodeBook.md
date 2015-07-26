This CodeBook breifly describes the data used and process.  A full description is available at the site from where the data was obtained:
http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 

#Various Parts of the R Script
Section 1. Merging the training and the test sets to create one data set.
After setting the source directory for the files, read into all the data files (text files)
Assign column names and merge to create one data set.

Section 2. Extracting only the measurements on the mean and standard deviation for each measurement.
Create a logcal vector that contains TRUE values for the ID, mean and stdev columns and FALSE values for the others. 
Subset this data to keep only the necessary columns.

Section 3. Using descriptive activity names to name the activities in the data set.
Merge data subset with the activityType table to inlude the descriptive activity names.

Section 4. Labeling the data set with descriptive activity names.
Use gsub function for pattern replacement to clean up the data labels.

Section 5. Creating the tidy data set with the average of each variable for each activity and each subject.
Finally, a data set with the average of each veriable for each activity and subject is produced.
