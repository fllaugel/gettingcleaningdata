CodeBook


The data files used
README.txt

features_info.txt: Shows information about the variables used on the feature vector.

features.txt: List of all features.

activity_labels.txt: Links the class labels with their activity name.

X_train.txt: Training set.

y_train.txt: Training labels.

x_test.txt: Test set.

y_test.txt': Test labels.


Transformation details

There are 5 parts:

Merges the training and the test sets to create one data set.
Extracts only the measurements on the mean and standard deviation for each measurement.
Uses descriptive activity names to name the activities in the data set
Appropriately labels the data set with descriptive activity names.
Creates a second, independent tidy data set with the average of each variable for each activity and each subject.
How run_analysis.R implements the above steps:

Require reshapre2 and data.table librareis.
Load both test and train data
Load the features and activity labels.
Extract the mean and standard deviation column names and data.
Process the data. There are two parts processing test and train data respectively.
Merge data set.
