---
title: "LightGBM"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-09
toc: true
---
## Understanding LightGBM
What is LightGBM (LGBM)?

LGBM is an ensemble algorithm which is constructed from decision tree models. Decision trees are added one at a time to the ensemble and fit in order to correct the prediction errors made by previous models. In order to train the model, gradient descent is used to optimize the loss function. Basically, LGBM involves 3 elements:

- A loss function to be optimized: depend on the task (classification or regression)
- A weak learner to make prediction: in general, decision tree is being used as a weak learner. Trees are split to minimize the impurity criterion.
- An additive model to which we will add decision trees (weak learners) for minimization: decision trees are added one at a time while keeping existing trees (or sub-models) in the model unchanged. To minimize the loss when adding trees, gradient descent procedure is applied. To perform the gradient descent, we add a tree to the model to correct or improve the incorrect prediction done by the sub-models, which then results in reducing the loss. When a defined number of trees are added or the loss reaches an acceptable level or no longer improves on a validation dataset, the training stops.

## Practical
LightGBM from Scikit Learn can both work on regression and classification. One major advantage is that it can handle categorical variables itself. You just need to convert the type of categorical variables into "category".

## References
Link: 
1. [https://towardsdatascience.com/understanding-random-forest-58381e0602d2][https://towardsdatascience.com/understanding-random-forest-58381e0602d2]

[https://towardsdatascience.com/understanding-random-forest-58381e0602d2]: https://towardsdatascience.com/understanding-random-forest-58381e0602d2
