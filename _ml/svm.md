---
title: "Support Vector Machines"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-10
categories:
  - ml
tags:
  - regression
  - machine learning
toc: true
mathjax: true
---
## Understanding Support Vector Machines (SVM)
The main criteria of SVM is to maximize the margin between the points and the hyperplane.

### SVM with Liear Separator
For $$x \in R^p, h(x) = sign(w^Tx+b)$$. The equation $$w^Tx+b = 0$$ defines the hyperplane in the euclidean space $$R^p$$ previously mentionned.

As in its name, this version of SVM works if the data are linearly separable. What if the data are not then?

### Non-linear SVM and Kernel
This is when the data are not linearly separable. The idea is to project the data to a feature space using a feature map. One major advantage is that we can associate this feature map to a PDS kernel (Moore-Aronzajn Theorem 1950) and with this kernel, we can calculate the projection in feature space directly in the input space without working in the feature space (this trick works with canonical feature map: $$\phi(x) = k(.,x)$$ and associated Hilbert Space (called reproducing Hilbert space)).

## Practical
- There are 3 types of kernel: Linear, Polynomial and Gaussian kernel.
- In general, data should be all numerical. 
- Fitting in general takes some time and can be overfit if not careful enough.

## References
Link: 
1.
