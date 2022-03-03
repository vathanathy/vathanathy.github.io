---
title: "Decision Tree"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-16
categories:
  - Mlog
tags:
  - classifcation
toc: true
---
## Understanding Decision Tree
The main idea of decision tree is to look for feature and the split threshold that allows to minimize an impurity criterion. Differently put, it seeks for feature and split threshold that allows it to split observations in a way that the resulting groups are as different from each other as possible while keeping those in the same group as similar to each other as possible.

During the split, decision tree considers all the features and choose the one that minimize an impurity criterion.

## Practical
- In general, data should be all numerical. 
- For optimal result, the model should be reinitialized when train on new data.

## References
Link: 
1. [https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data][https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data]

[https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data]: https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data
