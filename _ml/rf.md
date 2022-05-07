---
title: "Random Forest"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-09
<!-- categories:
  - ml
tags:
  - Post Formats
  - readability
  - standard -->
toc: true
---

## Understanding Random Forest

Random Forest is built based on a large number of individual decision tree which operates together. Each tree of the random forest returns a class prediction and the class with the majority vote will be the return value of the model. Random Forest is known as a bagging method or Bootstrap Aggregation. Given a sample of size N, this essentially means that for each tree, we build:
– Train dataset: a sample of size N is constructed from a randomly sample with replacement. For instance, if our sample is [1,2,3,4,5], then we may give to one of the trees [1,1,3,4,4] as training sample. Both samples have the same size, but different in content.
– Feature randomness: differently from decision tree where we consider all features and choose the one that minimizes an impurity criterion, here we pick one feature out of a random subset of features. This will induce the variation from one tree to another and therefore, result in lower correlation across trees and more diversity.

At the end, the result to be returned from the random forest is the majority votes by trees.

## Practical
- In general, data should be all numerical. 
- Facing new data, the model should be reintialized and retrained to assure optimal result.

## References
Link: 
1. [https://towardsdatascience.com/understanding-random-forest-58381e0602d2][https://towardsdatascience.com/understanding-random-forest-58381e0602d2]
2. [https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data][https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data]

[https://towardsdatascience.com/understanding-random-forest-58381e0602d2]: https://towardsdatascience.com/understanding-random-forest-58381e0602d2
[https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data]: https://www.quora.com/Say-I-have-trained-a-Random-Forest-and-want-to-deploy-it-to-make-predictions-online-How-do-I-update-it-with-the-arrival-of-new-data
