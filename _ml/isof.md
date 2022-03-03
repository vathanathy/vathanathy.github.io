---
title: "Isolation Forest"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-09
categories:
  - ml
tags:
  - unsupervised
  - machine learning
toc: true
---
## Understanding Isolation Forest
What is Isolation Forest ? How does it work ?

Isolation Forest is an unsupervised ensemble method. It is built based on Decision Trees. The main application is on anomalies detection. The main assumption in building this method is the fact that we assume that anomalies are few and different and can be easily isolated. The training process is as followed:
1. For a given dataset, we randomly sample a subset and assign it to a binary tree.
2. In order to build the tree, we start by first selecting a random feature (from the set of all features). Then, we select a random threshold (any value in the range of minimum and maximum values of the selected feature).
3. If the value of a data point is less than the selected threshold, it goes to the left branch, else it goes to the right. And thus, a node is split into the left and the right branches.
4. The process described above from step 2 is continued recursively until each data point is completely isolated or until max depth (if defined) is reached.

When the training is complete, an ensemble of trees (Isolation Forest) is created. In order to calculate the anomaly score, a data point will go through all the trees which were trained earlier. The anomaly score for each data point is calculated based on the depth of the tree needed to arrive at that point. The score is the sum of the depth obtained from each of the trees. A score of -1 is labeled as anomalies and 1 as normal points based on the contamination parameter (proportion of anomalies present in the data).

## Practical
This is specifically about the Isolation Forest model implemented by Scikit Learn. Data in general contain categorical and numerical variables. Categorical variables need to be converted into numerical ones, either one-hot encoding, label encoder or ordinal encoder.   

## References
Link: 
1. ??
