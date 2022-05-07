---
title: "Linear Regression"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-10
<!-- categories:
  - ml
tags:
  - regression
  - machine learning -->
toc: true
mathjax: true
---
## Understanding Linear Regression
Linear Regression basically means trying to find the best fit line for the numserical data.

### Ordinary Least Squares (OLS)
OLS is one of the variety for linear regression. The model fits a model of form $$y = ax + b$$ and trying to minimize the Mean Square Error. OLS considers data as a matrix and uses linear algebra to solve for optimal values. Scikit Learn linear regressor implements with this configuration.

### Linear Regression with Gradient Descent
This is another variety. The optimization process is iterative following the steepest direction provided from the derivative of loss in funtion of parameters. This iterative process can be 3 types:
- Batch gradient descent: use all data for one iteration
- Stochastic gradient descent: use one data instance for one iteration
- Mini-batch gradient descent: use a batch of data for one iteration (commonly used)

## Practical
In general, data should be all numerical. Good practise is to plot the linearity between the target and all the numerical variables to see if there is any. If not, we should consider other models. On the other hand, I believe OLS model does not need to standardized data whereas Gradient Descent model needs standardized data, just like any other gradient descent models.

## References
Link: 
1. [https://towardsdatascience.com/linear-regression-simplified-ordinary-least-square-vs-gradient-descent-48145de2cf76][https://towardsdatascience.com/linear-regression-simplified-ordinary-least-square-vs-gradient-descent-48145de2cf76]
2. [https://towardsdatascience.com/https-medium-com-chayankathuria-optimization-ordinary-least-squares-gradient-descent-from-scratch-8b48151ba756][https://towardsdatascience.com/https-medium-com-chayankathuria-optimization-ordinary-least-squares-gradient-descent-from-scratch-8b48151ba756]
3. [https://medium.com/@ga3435/understanding-comparing-linear-regression-using-ols-and-gradient-descent-de237c14516][https://medium.com/@ga3435/understanding-comparing-linear-regression-using-ols-and-gradient-descent-de237c14516]
4. [https://stats.stackexchange.com/questions/484664/does-linear-regression-needs-target-variable-to-be-normally-distributed-glm-co][https://stats.stackexchange.com/questions/484664/does-linear-regression-needs-target-variable-to-be-normally-distributed-glm-co]
5. [https://machinelearningmastery.com/linear-regression-for-machine-learning/][https://machinelearningmastery.com/linear-regression-for-machine-learning/]


[https://towardsdatascience.com/linear-regression-simplified-ordinary-least-square-vs-gradient-descent-48145de2cf76]: https://towardsdatascience.com/linear-regression-simplified-ordinary-least-square-vs-gradient-descent-48145de2cf76
[https://towardsdatascience.com/https-medium-com-chayankathuria-optimization-ordinary-least-squares-gradient-descent-from-scratch-8b48151ba756]: https://towardsdatascience.com/https-medium-com-chayankathuria-optimization-ordinary-least-squares-gradient-descent-from-scratch-8b48151ba756
[https://medium.com/@ga3435/understanding-comparing-linear-regression-using-ols-and-gradient-descent-de237c14516]: https://medium.com/@ga3435/understanding-comparing-linear-regression-using-ols-and-gradient-descent-de237c14516
[https://stats.stackexchange.com/questions/484664/does-linear-regression-needs-target-variable-to-be-normally-distributed-glm-co]: https://stats.stackexchange.com/questions/484664/does-linear-regression-needs-target-variable-to-be-normally-distributed-glm-co
[https://machinelearningmastery.com/linear-regression-for-machine-learning/]: https://machinelearningmastery.com/linear-regression-for-machine-learning/
