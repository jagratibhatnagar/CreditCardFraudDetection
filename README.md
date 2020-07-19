# CreditCardFraudDetection

                                               Project 2:   Credit Card Fraud Detection

__Problem Statement:__ Project to detect fraudulent transactions using a dataset of nearly 28,500 credit card transactions and multiple unsupervised anomaly detection algorithms, and to identify transactions with a high probability of being credit card fraud. 

Dataset __*creditcard.csv*__ has been taken from: __*https://www.kaggle.com/mlg-ulb/creditcardfraud*__

__Steps Involved:__

   1.	Importing Necessary Libraries
    
   2.	Loading dataset
    
   3.	Data Exploring:
    Exploring the dataset to gain an understanding of the type, quantity, and distribution of data in our dataset and Determining number of fraud cases in dataset.
    
   4.	Data Visualization:
   
    To gain a better understanding of the underlying distribution of data in our data set  following Visualization techniques are used in this project:
   
             	Histogram for each parameter
             
             	Correlation matrices 
   
   5.	Deploying Machine Learning Algorithms 
   
   In this project, the following two machine learning algorithms are used:
    
   •	__Local Outlier Factor (LOF:__
   
   The anomaly score of each sample is called Local Outlier Factor. It measures the local deviation of density of a given sample with respect to its neighbors. It is local in that the anomaly score depends on how isolated the object is with respect to the surrounding neighborhood.

   •	__Isolation Forest Algorithm:__
   
   The IsolationForest ‘isolates’ observations by randomly selecting a feature and then randomly selecting a split value between the maximum and minimum values of the selected feature.
   Since recursive partitioning can be represented by a tree structure, the number of splittings required to isolate a sample is equivalent to the path length from the root node to the terminating node.
   This path length, averaged over a forest of such random trees, is a measure of normality and our decision function.
   Random partitioning produces noticeably shorter paths for anomalies. Hence, when a forest of random trees collectively produce shorter path lengths for particular samples, they are highly likely to be anomalies.
    
   why the classification accuracy for these algorithms can be misleading is investigated using following metrics:
    
                 	Precision
                 	Recall
                 	F1-scores

__Output:__ Accuracy score for Isolation Forest ( 0.9975) is greater than that of Local Outlier Factor (0.99659 )
