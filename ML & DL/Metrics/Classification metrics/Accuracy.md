**Accuracy** is a [[metric]] measured how often predictions equal labels. Accuracy as describing a combination of both types of observational error (random and systematic), so high accuracy requires both high precision and high trueness

#### Evaluation Function:
$$
Accuracy = \frac{1}{n}\sum_{i=1}^n[\hat y_i = y_i]
$$

#### Derivative of a Function:
<h5 align='center' style='color:red'>Loss function is not implemented</h5>

#### Pros and Cons:

* Pros:
	* Easy to understand and interpret
	* Useful when the classes are balanced
	* Can provide a quick and general idea of how well a model is performing
* Cons:
	* Bad for imbalanced data
	* Does not take account False Negative (FN) and False Positive (FP) values