**Huber loss** is a [[metric]] used in robust regression, that is less sensitive to outliers in data than the squared error loss. A variant for classification is also sometimes used


#### Evaluation Function:
$$
HUBER = \begin{cases} \frac{1}{2}(y-\hat y)^2, & \mbox{for } |y - \hat y| \leq \delta \\ \delta\cdot(|y-\hat y| - \frac{1}2\delta), & \mbox{otherwise.} \end{cases}
$$

#### Derivative of a Function:
$$
\delta HUBER = \begin{cases} \hat y - y, & \mbox{for } |y - \hat y| \leq \delta \\ \delta\cdot sgn(\hat y - y), & \mbox{otherwise.} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* Very robust to outliers
	* -
* Cons:
	* -