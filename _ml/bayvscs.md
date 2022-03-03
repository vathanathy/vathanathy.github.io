---
title: "Bayesian vs Classical Statistic"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-02-09
categories:
  - Blog
  - Mlog
tags:
  - bayes
  - statistic
toc: true
---

This is considered to be what I understand from a google search for the differences between Bayesian and Classical statistic method.

Statistical method is also called as an "objective" method, because the main idea is that you have some data and then you impose a model on that data. The following process for example Linear Regression, is that you try to understand the underlying paramters which in this case W and b.

Bayesian method is more complicated than that. It is known as a "subjective" method. This subjective word comes from the fact that you have a prior distribution/knowledge to the data/observations you currently have. Within this prior distribution/knowledge, you try to predict the underlying truth. One good example given in the blog I read, you went to a zoo. You observed 3 lions, 2 tigers and 1 bear. You want to know the probability of observing a bear (posterior) when you come next time knowing that there are only three types of animals and knowing from your friend who visited the zoo before that there is an equal number of each animal (prior). You can consider this prior as belief. Obviously, this prior knowledge would help you in estimating your posterior distribution.


Link: 
1. [https://towardsdatascience.com/estimating-probabilities-with-bayesian-modeling-in-python-7144be007815][https://towardsdatascience.com/estimating-probabilities-with-bayesian-modeling-in-python-7144be007815]
2. [https://www.quora.com/What-are-the-differences-a-beginner-must-know-about-classical-vs-Bayesian-statistics][https://www.quora.com/What-are-the-differences-a-beginner-must-know-about-classical-vs-Bayesian-statistics]


[https://www.quora.com/What-are-the-differences-a-beginner-must-know-about-classical-vs-Bayesian-statistics]: https://www.quora.com/What-are-the-differences-a-beginner-must-know-about-classical-vs-Bayesian-statistics
[https://towardsdatascience.com/estimating-probabilities-with-bayesian-modeling-in-python-7144be007815]: https://towardsdatascience.com/estimating-probabilities-with-bayesian-modeling-in-python-7144be007815
