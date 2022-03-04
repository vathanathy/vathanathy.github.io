---
title: "Metrics"
excerpt_separator: "<!--more-->"
last_modified_at: 2022-03-02
categories:
  - ml
tags:
  - classifcation
  - machine learning
toc: true
mathjax: true
---
## Understanding metrics
For classification problem in the machine learning community, there are 4 main metrics being used: accuracy, precision, recall and F1. We will state the differences between these metrics. However, it is worth look at confusion matrix first.

|       | 	     | Predicted       |                 | 
|       |            | Negative        | Positive        | 
|Actual | Negative   | True Negative   | False Positive  |
|       | Positive   | False Negative  | True Positive   |

<!-- <img src="{{ site.url }}{{ site.baseurl }}/assets/images/metric.png" alt="" class="full"> -->

### Accuracy
\\begin{align}
    Accuracy & =  \frac{\text{True Negative + True Positive}}{\text{True Negative + True Positive + False Positive + False Negative}} \\\\\\\\
    & = \frac{\text{Total correctly predicted}}{\text{All predictions}}
\\end{align}  

As seen in the formula, accuracy is the metric showing the model being correct and precise. However, this means that the metric is dominated by the correct prediction. This might not be always interesting to use in order to evaluate the model as sometimes, the mis-classified actual positive can be costly, if positive means someone carrying highly contagious virus, or a fraud case or a terrorist attack.


### Precision
\\begin{align}
	Precision & =  \frac{\text{True Positive}}{\text{True Positive + False Positive}} \\\\\\\\
	& = \frac{\text{True Positive}}{\text{Total predicted positive}}
\\end{align}  
According the formula, we can see that Precision metric measures how precise the model is out of the predicted positive by calculating the ratio of how many of predicted positive are actually positive. This metric is practical for the case where False Positive are costly and where we want to avoid False Positive as much as possible, for instance _spam email detection_ (positive = spam, negative = non-spam). A non-spam email detected as a spam email might be annoying to users.

### Recall
\\begin{align}
	Recall & =  \frac{\text{True Positive}}{\text{True Positive + False Negative}} \\
	& = \frac{\text{True Positive}}{\text{Total actual positive}}
\\end{align}  
Here, Recall measures the ratio of how many of Actual Positive the model predicts correctly. Similarly, this metric is useful to evaluate the model when we want to avoid False Negative as much as possible. As example, this should be the metric for the use case of fraud detection and patient infected by highly contagious virus detection. If a fraudulent action is predicted as non-fraudulent, or a infected patient is predict as healthy, then you can see the consequence behind.

### F1-score
\\begin{align}
	F1 & =  2 * \frac{\text{Precision * Recall}}{\text{Precision + Recall}} \\
	& =  \frac{\text{True Positive}}{\text{True Positive} + \frac{1}{2}(\text{False Positive + False Negative})}
\\end{align}
Differently from Recall and Precision, instead of putting high cost on one of errors, F1 score is measured based on both False Positive and False Negative. Either of these errors being too high will result in bad score. Therefore, F1 score can measure the balance of errors out of a model.

## References
Link: 
