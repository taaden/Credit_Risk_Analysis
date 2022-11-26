# Credit_Risk_Analysis

## Overview of the analysis

  The purpose of this analysis is to bulid and evaluate several machine learning models to predict credit risk,
  using the credit card credit dataset from LendingClub, a peer-to-peer lending services company.
  
  The analysis will entails:
  * Oversample the data using the RandomOverSampler and SMOTE algorithms, 
    and undersample the data using the ClusterCentroids algorithm.
    
  * Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
  
  * Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
  
Finally we will evaluate the performance of these models and make a recommendation on their usage to predict credit risk.

### Results

  The Balanced Accuracy Score and The Precision and Recall Scores of all six machine learning models
  
 * RandomOverSampler model

![image](https://user-images.githubusercontent.com/64270455/204111570-a9b86690-7d9a-4369-bf1d-7694e8f0c372.png)


![image](https://user-images.githubusercontent.com/64270455/204111625-ced319c6-c973-406b-b316-1d7b66af998a.png)


![image](https://user-images.githubusercontent.com/64270455/204111658-09938ab2-1a9b-4546-a8f3-03089e19af99.png)

 In this Model,the balanced accuracy score is 65%, the high_risk precision is about 1%  with 62% sensitivity which makes a F1 of 2%.
 There is the high number of the low_risk population,with the  precision is almost 100% with a sensitivity of 68%.
