# Credit_Risk_Analysis

![image](https://user-images.githubusercontent.com/94503395/164357743-4a254de0-c49a-4910-b730-88e2035907bb.png)

## Overview of the analysis: 

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.



## Results: Six Models outputs.

* The naive random oversampling algorithm result in a balanced accuracy score of 0.657. The precision score was 1.0 for predicting low risk, also extremely low for predicting high risk (0.01). 

![image](https://user-images.githubusercontent.com/94503395/164951210-78adf743-dcf9-4ee9-8b69-2fdee401be53.png)
![image](https://user-images.githubusercontent.com/94503395/164951409-fdd87f7a-48be-4db3-b13a-0400ec7f30e9.png)

* The SMOTE algorithm result in a balanced accuracy score of 0.662. The precision for predicting high and low risk was 
the same as the naive random oversampling algorithm. The recall scores were 0.63 and 0.69 for high and low risk.

![image](https://user-images.githubusercontent.com/94503395/164951461-4e5ef126-a2c2-45c0-b295-cd259673a197.png)
![image](https://user-images.githubusercontent.com/94503395/164951473-b86f1542-4e15-454a-8c5a-3a1173bd90f1.png)

* The Cluster Centroids algorithm result in a resulted in a balanced accuracy score of 0.544. 

![image](https://user-images.githubusercontent.com/94503395/165651447-c3aad448-3e9d-4a94-9949-4c0df008e8ab.png)

* The SMOTEENN algorithm result in a balanced accuracy score of 0.687. The precision for predicting high and low risk was the same as all the previous algorithms. The recall scores is 0.80 and 0.57 for high and low risk.

![image](https://user-images.githubusercontent.com/94503395/164952048-c5e4cdff-5680-4420-a45d-0da5b28a5d5c.png)

* The Balanced Random Forest Classifier result in a resulted in a balanced accuracy score of 0.788.

![image](https://user-images.githubusercontent.com/94503395/164952178-33b97fd6-e9dc-4d61-a33f-d9678d772d86.png)

* The Easy Ensemble Classifier result in balanced accuracy score of 0.93. The precision and recall scores for predicting high and low risk were the same as the Balanced Random Forest Classifier.

![image](https://user-images.githubusercontent.com/94503395/164952295-d0101bcb-8b04-4527-9818-8a7c768ddb3c.png)
![image](https://user-images.githubusercontent.com/94503395/164952319-e25d0cd8-9474-411a-9973-82d3976b240b.png)


## Summary: 
In conclusion credit risk is a very difficult formula to predict, I would recommend to use the Easy Ensemble Classsifer because it had the highest balanced accuracy score of 0.93, although the company should be aware of the implications of the precision scores. The precision score of 0.09 means that a high risk classification is not very reliable.  I would advise not to use these algorithms, because it would put creditors at a too reat of a risk being unable to accurately predict the hig-risk clients.
