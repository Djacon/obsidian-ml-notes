**Squared Hinge loss** is a modified version of [[metric]] of the [[hinge loss]] function, it commonly used in [[support vector machines]]. Its primary advantage is that it is a smooth, continuous function that can be easily differentiated. This makes it easier to optimize using gradient-based methods

#### Evaluation Function:
$$
HINGE_2 = \begin{cases} 0, & \mbox{if } 1-y\cdot\hat y \leq 0 \\ (1-y\cdot\hat y)^2, & \mbox{otherwise} \end{cases}
$$

#### Derivative of a Function:
$$
\delta HINGE_2 = \begin{cases} 0, & \mbox{if } 1-y\cdot\hat y \leq 0 \\ 2y\cdot(y\cdot\hat y-1), & \mbox{otherwise} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* Easy to differentiate
	* Penalizes misclassifications more strongly than regular **hinge loss**
	* Seeks to maximize the margin between positive and negative examples
* Cons:
	* Binary classification only
	* Sensitive to outliers
	* May be overfitting to the training data