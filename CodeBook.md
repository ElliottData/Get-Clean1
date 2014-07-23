The Data

   The data for this project was collected from the accelerometers from the Samsung Galaxy S smartphone. 
   The original data I used is contained in 7 seperete files: 
   
  xtest.txt-             a test dataset with observed measurements 
  
  ytest.txt-             a dataset assinging activities to the test observations 
  
  xtrain.txt-            a training dataset with observed measurements 
  
  ytrain.txt-            a dataset of the activities for the training data 
  
  subject_test.txt-      a dataset listing the subjects for each of the test observations
  
  subject_training.txt - a dataset listing the subjects for each of the training observations
  
  features.txt-          a list of all the feastures(the names for all the meaurements)
   
More information pertaining to the source of the data can be found here: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 


The Transformation & Cleanup

The script run_analysis.R works reading in training and test observations, then merges the two sets together. The same is done for the datasets containing training and test subject information as a seperate data frame, then training and test activity observations are read in and combined into their own data frame as well. After this the list of features are applied to the appropiate columns as header names for the observerd measurements.


At this point the features containing mean and standard deviation measuresment are pulled as a subset of data. Then changes to the feature names were made to make the names more easily readable and R friendly. These changes included:

   -Replacing the abbreviation "t" with "time"
   -Removing the "-" and "()" characters
   -Replacing the abbreviation "f" with 'freq" (frequency)
   -Replacing "std" with StdDev (standard deviation)
   -Replacing "mean" with Mean (to maintain camel casing format)
   -Replacing "BodyBody" with "Body"(to correct a typo found in the original features dataset) 




The columns containing activity and subject are renamed as well.

