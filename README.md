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
  
 * RandomOverSampler Model

![image](https://user-images.githubusercontent.com/64270455/204111570-a9b86690-7d9a-4369-bf1d-7694e8f0c372.png)


![image](https://user-images.githubusercontent.com/64270455/204111625-ced319c6-c973-406b-b316-1d7b66af998a.png)


![image](https://user-images.githubusercontent.com/64270455/204111658-09938ab2-1a9b-4546-a8f3-03089e19af99.png)

 In this Model,the balanced accuracy score is 64%, the high_risk precision is about 1%  with 69% sensitivity and a F1 of 2%.
 There is a high number of the low_risk population,with the  precision is almost 100%, a sensitivity of 59% and F1 of 74%.
 
  * SMOTE Model
  
  ![image](https://user-images.githubusercontent.com/64270455/204115246-9d15d4c5-afdb-4cf5-bb6c-1a209d299133.png)


 ![image](https://user-images.githubusercontent.com/64270455/204115274-b55fdb99-b311-4fef-acbf-7ccbd6bd893a.png)

 
 ![image](https://user-images.githubusercontent.com/64270455/204115334-f6395084-a9bd-4583-aa86-8f72d3f5a300.png)
 
 The results here are pretty similar to the previous model,the balanced accuracy score is 66%.
 The high_risk precision is about 1% , with 63% sensitivity and a F1 of 2% .
 There is a high number of the low_risk population,with a  precision of almost 100%, a sensitivity of 69% and F1 of 82%.
 There is a reduction in the high risk sensitivity compared to the previous model while the low risk sensitivity increased.
 
   * ClusterCentroids Model
 
 ![image](https://user-images.githubusercontent.com/64270455/204116138-7b2929a0-a0ea-4e3c-ba73-f608d0ecdff5.png)


 ![image](https://user-images.githubusercontent.com/64270455/204116156-6958dcfd-714b-4fe7-8b56-192d5b228d1e.png)
 
 
 ![image](https://user-images.githubusercontent.com/64270455/204116181-633605db-2260-478e-9d53-36ffa70f280e.png)

 In this model,the balanced accuracy score is low 54%, the high_risk precision is about 1%  with 69% sensitivity and a F1 of 1%.
 There is a high number of the low_risk population,with the  precision is almost 100%, a very low sensitivity of 40% and F1 of 57%.
 
   * SMOTEENN Model
 
 ![image](https://user-images.githubusercontent.com/64270455/204116419-48a34c5e-ade5-4db8-aa8e-ee343ac03242.png)


 ![image](https://user-images.githubusercontent.com/64270455/204116452-25d64e2f-8c02-4487-99f7-389114076ff4.png)


 ![image](https://user-images.githubusercontent.com/64270455/204116464-a45d3d07-56bf-479c-87d8-d771439f08b2.png)
 
 In this Model,the balanced accuracy score is 64%, the high_risk precision is about 1%  with 70% sensitivity and a F1 of 1%.
 There is a high number of the low_risk population,with the  precision is almost 100%, a sensitivity of 57% and F1 of 73%.
 This model result is very similar to the RandomOverSampler Model.
 
   * Balanced Random Forest Classifier Model
 
 
 ![image](https://user-images.githubusercontent.com/64270455/204116674-440eb69a-ec32-4d60-bc9a-fdad78004c43.png)
 
 
 ![image](https://user-images.githubusercontent.com/64270455/204116727-57acaad9-fd48-46a1-b39a-58b1de113e1e.png)


 ![image](https://user-images.githubusercontent.com/64270455/204116752-c615fb6f-cd04-4615-a112-2c0ed4b54cb8.png)
 
 The balanced accuracy score improved to about 79%.The high_risk precision is still low at 4%  with 67% sensitivity and a F1 of 7%.
 The low_risk sensitivity is now 91% with 100% presicion and F1 is 95%.
  
   * EasyEnsembleClassifier Model
 
 ![image](https://user-images.githubusercontent.com/64270455/204117002-a5e74959-8f0a-40b9-8b81-e602541e3f76.png)
 
 
 ![image](https://user-images.githubusercontent.com/64270455/204117029-7cf01c11-2486-457f-a864-79677e567bd9.png)

  The balanced accuracy score improved to about 93%.The high_risk precision is still low at 7%  with 91% sensitivity and a F1 of 14%.
  The low_risk sensitivity is now 94% with 100% presicion and F1 is 97%.
  
  #### Summary
    The Ensemble model shows a lot of improvement on the sensitivity of the high risk credits while all 
    the models used in this analysis show weak precision in determining if a credit risk is high.

    The EasyEnsembleClassifier model shows a recall of 92% so it detects almost all high risk credit 
    but with a low precision,as a reslut a lot of low risk credits are still falsely detected as high risk 
    which  might be denied of loan thereby missing those business opportunities.At the same time, the EasyEnsembleClassifier
    model has 100% precision predicting low risk at 94% sensitivity.
    
    For these reasons I would recommend that the banks use the EasyEnsembleClassifier model to predict credit
    risk as it is able to screen out high risk and predict with high precision low credit risk.
    
  
 


 
 

 



