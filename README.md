# Discerning Seizure Activity From EEG

## September 2021
## Lincoln Kartchner

Epilepsy is a disorder of the central nervous system that involves abnormal electrical brain activity and the occurence of seizures. Approximately 3.4 million people in the U.S. have epilepsy. 

This project uses EEG data from the UCI Machine Learning Repository to analyze the effectiveness of various supervised classification algorithms in detecting seizures. 

The consists of EEG time-series data from 23-second recordings gathered on 500 subjects. The original dataset contains five different classifications, and these were simplified to reflect a binary, 0 (no seizure) and 1 (seizure), classification.

After the data simplification, Principal Component Analysis was performed for dimensionality reduction, having identified that the majority of the variance was captured in the first 50 eigenvectors of the dataset. After this, five different models were fit and tested on the data: K-Nearest Neighbors, Random Forest, Support Vector Machine, Gaussian Naive Bayes and a Long Term Short Memory Network. 

Each classifier had a 10-fold cross validation accuracy score of greater than 95%, with the Random Forest and the Support Vector Machine producing the most accurate predictions of >97%. The SVM had the highest sensitivity (97.6%) while the K-NN model had the highest specificity (99.9%). 

The models built in this project were simple, and are a way of demonstrating the capability of various Python Machine Learning tools and libraries more than anything. However, the results of this project highlight that various machine learning algorithms may prove useful in the detection of seizure activity from EEG data.

This repository contains the .ipynb code used to perform the analysis, which can be opened, viewed and edited in Google Colab.
