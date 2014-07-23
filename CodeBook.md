
The Transformation & Cleanup

The script run_analysis.R works by reading in training and test observations, then merges the two sets together. The same is done for the datasets containing training and test subject information as a separate data frame, then training and test activity observations are read in and combined into their own data frame as well. After this the list of features are applied to the appropriate columns as header names for the observed measurements.


At this point the features containing mean and standard deviation measurement are pulled as a subset of data. Then changes to the feature names were made to make the names more easily readable and R friendly. These changes included:

   -Replacing the abbreviation "t" with "time"
   
   -Removing the "-" and "()" characters
   
   -Replacing the abbreviation "f" with 'freq" (frequency)
   
   -Replacing "std" with StdDev (standard deviation)
   
   -Replacing "mean" with Mean (to maintain camel casing format)
  
   -Replacing "BodyBody" with "Body"(to correct a typo found in the original features dataset) 

The columns containing activity and subject are renamed as well, replacing the default names given by the system.

As a final step the script summarizes the data by providing the average measurement for each feature, for each of the activities, by subject. 

The Data

Here are the variables in the resulting data set.

Variable                     Value    
   Subject                    : ID# of Subject, ranging 1-30
   Activity                   : Type of activity(WALKING, WALKING UPSTAIRS,
                                WALKING DOWNSTAIRS, SITTING, STANDING,LAYING) 
   timeBodyAccMeanX           :  mean average of for this feature  
   timeBodyAccMeanY           :  mean average of for this feature  
   timeBodyAccMeanZ           :  mean average of for this feature  
   timeBodyAccStdDevX         :  mean average of for this feature  
   timeBodyAccStdDevY         :  mean average of for this feature  
   timeBodyAccStdDevZ         :  mean average of for this feature  
   timeGravityAccMeanX        :  mean average of for this feature  
   timeGravityAccMeanY        :  mean average of for this feature  
   timeGravityAccMeanZ        :  mean average of for this feature  
   timeGravityAccStdDevX      :  mean average of for this feature  
   timeGravityAccStdDevY      :  mean average of for this feature  
   timeGravityAccStdDevZ      :  mean average of for this feature  
   timeBodyAccJerkMeanX       :  mean average of for this feature  
   timeBodyAccJerkMeanY       :  mean average of for this feature  
   timeBodyAccJerkMeanZ       :  mean average of for this feature 
   timeBodyAccJerkStdDevX     :  mean average of for this feature  
   timeBodyAccJerkStdDevY     :  mean average of for this feature  
   timeBodyAccJerkStdDevZ     :  mean average of for this feature  
   timeBodyGyroMeanX          :  mean average of for this feature  
   timeBodyGyroMeanY          :  mean average of for this feature
   timeBodyGyroMeanZ          :  mean average of for this feature 
   timeBodyGyroStdDevX        :  mean average of for this feature  
   timeBodyGyroStdDevY        :  mean average of for this feature  
   timeBodyGyroStdDevZ        :  mean average of for this feature 
   timeBodyGyroJerkMeanX      :  mean average of for this feature 
   timeBodyGyroJerkMeanY      :  mean average of for this feature 
   timeBodyGyroJerkMeanZ      :  mean average of for this feature  
   timeBodyGyroJerkStdDevX    :  mean average of for this feature  
   timeBodyGyroJerkStdDevY    :  mean average of for this feature  
   timeBodyGyroJerkStdDevZ    :  mean average of for this feature  
   timeBodyAccMagMean         :  mean average of for this feature  
   timeBodyAccMagStdDev       :  mean average of for this feature  
   timeGravityAccMagMean      :  mean average of for this feature  
   timeGravityAccMagStdDev    :  mean average of for this feature  
   timeBodyAccJerkMagMean     :  mean average of for this feature 
   timeBodyAccJerkMagStdDev   :  mean average of for this feature  
   timeBodyGyroMagMean        :  mean average of for this feature  
   timeBodyGyroMagStdDev      :  mean average of for this feature  
   timeBodyGyroJerkMagMean    :  mean average of for this feature  
   timeBodyGyroJerkMagStdDev  :  mean average of for this feature 
   freqBodyAccMeanX           :  mean average of for this feature  
   freqBodyAccMeanY           :  mean average of for this feature 
   freqBodyAccMeanZ           :  mean average of for this feature 
   freqBodyAccStdDevX         :  mean average of for this feature  
   freqBodyAccStdDevY         :  mean average of for this feature  
   freqBodyAccStdDevZ         :  mean average of for this feature  
   freqBodyAccMeanFreqX       :  mean average of for this feature  
   freqBodyAccMeanFreqY       :  mean average of for this feature  
   freqBodyAccMeanFreqZ       :  mean average of for this feature  
   freqBodyAccJerkMeanX       :  mean average of for this feature  
   freqBodyAccJerkMeanY       :  mean average of for this feature  
   freqBodyAccJerkMeanZ       :  mean average of for this feature  
   freqBodyAccJerkStdDevX     :  mean average of for this feature  
   freqBodyAccJerkStdDevY     :  mean average of for this feature  
   freqBodyAccJerkStdDevZ     :  mean average of for this feature  
   freqBodyAccJerkMeanFreqX   :  mean average of for this feature  
   freqBodyAccJerkMeanFreqY   :  mean average of for this feature  
   freqBodyAccJerkMeanFreqZ   :  mean average of for this feature  
   freqBodyGyroMeanX          :  mean average of for this feature  
   freqBodyGyroMeanY          :  mean average of for this feature  
   freqBodyGyroMeanZ          :  mean average of for this feature  
   freqBodyGyroStdDevX        :  mean average of for this feature  
   freqBodyGyroStdDevY        :  mean average of for this feature  
   freqBodyGyroStdDevZ        :  mean average of for this feature  
   freqBodyGyroMeanFreqX      :  mean average of for this feature  
   freqBodyGyroMeanFreqY      :  mean average of for this feature  
   freqBodyGyroMeanFreqZ      :  mean average of for this feature  
   freqBodyAccMagMean         :  mean average of for this feature  
   freqBodyAccMagStdDev       :  mean average of for this feature  
   freqBodyAccMagMeanFreq     :  mean average of for this feature 
   freqBodyAccJerkMagMean     :  mean average of for this feature  
   freqBodyAccJerkMagStdDev   :  mean average of for this feature 
   freqBodyAccJerkMagMeanFreq :  mean average of for this feature  
   freqBodyGyroMagMean        :  mean average of for this feature  
   freqBodyGyroMagStdDev      :  mean average of for this feature 
   freqBodyGyroMagMeanFreq    :  mean average of for this feature 
   freqBodyGyroJerkMagMean    :  mean average of for this feature 
   freqBodyGyroJerkMagStdDev  :  mean average of for this feature
  freqBodyGyroJerkMagMeanFreq :  mean average of for this feature  
