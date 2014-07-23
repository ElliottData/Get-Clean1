The Data

   The data for this project was collected from the accelerometers from the Samsung Galaxy S smartphone. 
   The original data I used is contained in 7 seperete files: 
   
  xtest.txt-             a test dataset with observed measurements 
  
  ytest.txt-             a dataset assinging activities to the test observations 
  
  xtrain.txt-            a training dataset with observations
  
  ytrain.txt-            a dataset of the activities for the training data 
  
  subject_test.txt-      a dataset listing the subjects for each of the test observations
  
  subject_training.txt - a dataset listing the subjects for each of the training observations
  
  features.txt-          a list of all the feastures(the names for all the meaurements)
   
More information pertaining to the source of the data can be found here: 

http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones 


The Transformation & Cleanup

The script run_analysis.R works reading in training and test observations, then merges the two sets together. The same is done for the datasets containing training and test subject information, then training and test activity observations anre read in and combined as well.
