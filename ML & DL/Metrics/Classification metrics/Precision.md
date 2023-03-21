**Precision** is a [[metric]] used in [[Machine Learning]] to evaluate the accuracy of a [[Classification]] model. It is defined as the ratio of true positives (TP) to the sum of true positives and false positives (FP). In other words, **Precision** is the proportion of truly positive to all classified as positive

#### Evaluation Function:
$$
\mbox{Precision} = \frac{\sum TP}{\sum TP+FP} = \frac{\sum_{i=1}^n[\hat y_i = y_i = n]}{\sum_{i=1}^n[\hat y_i = n]}
$$

#### Derivative of a Function:
<h5 align='center' style='color:red'>Loss function is not implemented</h5>

#### Pros and Cons:

* Pros:
	* Correctly identifying positive samples
	* Helps to identify the False Positives (FP)
	* Easy to calculate and interpret, making it widely used metric
* Cons:
	* Sensitive to imbalanced data
	* Does not take account False Negative (FN) values
	* Is not useful when FN is high (in such case [[Recall]] is better option)

