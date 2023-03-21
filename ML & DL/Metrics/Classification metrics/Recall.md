**Recall** is a [[metric]] used in [[Machine Learning]] to measure the ability of a model to correctly identify all relevant instances or examples of a particular class in a dataset. In other words, **Recall** is the proportion of truly positives (TP) among all actual positives ($y_i = 1$) in a binary [[Classification]]

#### Evaluation Function:
$$
\mbox{Recall} = \frac{\sum TP}{\sum TP+FN} = \frac{\sum_{i=1}^n[\hat y_i = y_i = n]}{\sum_{i=1}^n[y_i = n]}
$$

#### Derivative of a Function:
<h5 align='center' style='color:red'>Loss function is not implemented</h5>

#### Pros and Cons:

* Pros:
	* Useful when FN is high
	* Helps to identify the False Negatives (FN)
	* Easy to calculate and interpret, making it widely used metric
* Cons:
	* Sensitive to imbalanced data
	* Does not take account False Positive (FP) values
	* Is not useful when FP is high (in such case [[Precision]] is better option)