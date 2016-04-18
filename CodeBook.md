The run_analysis.R script does the following things.

Read X_train.txt, y_train.txt and subject_train.txt from the "./data/train" folder and store them in trainData, trainLabel and trainSubject variables.

Read X_test.txt, y_test.txt and subject_test.txt from the "./data/test" folder and store them in testData, testLabel and testsubject variables.

Concatenate testData to trainData to "joinData". Concatenate testLabel to trainLabel to "joinLabel". Concatenate testSubject to trainSubject to "joinSubject".

Read features.txt from the "/data" folder and store the data in a variable called features.

Extract the measurements on the mean and standard deviation. 

Clean the column names of the subset. Remove the "()" and "-" symbols in the names, then make the first letter of "mean" and "std" a capital letter "M" and "S".

Read activity_labels.txt from the "./data"" folder and store the data in a variable called activity.

Clean the activity names in the second column of activity. Rewrite all names to lower cases.

Capitalize the letter after the underscore if there was an underscore between letters.

Transform the values of joinLabel based on the activity data frame.

Combine the joinSubject, joinLabel and joinData by column to "cleanedData". 

Write the cleanedData out to "merged_data.txt" file in current working directory.

Generate a second independent tidy data set with the average of each measurement for each activity and each subject. Calculate the mean of each measurement with the corresponding combination. So, after initializing the result data frame and performing the two for-loops, we get a 180x68 data frame.

Write the result out to "data_with_means.txt" file in current working directory.