**Log-Loss (aka Binary Cross-Entropy, BCE)** is a commonly used [[metric]] in binary [[classification]] problems. It measures the difference between the predicted probability (either 0 or 1) and the true binary label, by computing the negative log-likelihood of the predicted probability distribution

#### Evaluation Function:
$$
BCE = \frac{1}{n}\sum_{i=1}^n -(y_i\log(\hat y_i)\ + (1-y_i)\log(1-\hat y_i))
$$

#### Derivative of a Function:
$$
\delta BCE = \frac{1}{n}\sum_{i=1}^n \frac{\hat y_i - y_i}{\hat y_i\cdot(1 - \hat y_i)}
$$

#### Pros and Cons:

* Pros:
	* Easy to differentiate
	* Robust to imbalanced datasets
	* It can output predicted probabilities of belonging to a class, rather than just binary labels
* Cons:
	* Sensitive to outliers
	* Computationally expensive (because it use logarithm for prediction)
	* Not the best choice for multi-class classification