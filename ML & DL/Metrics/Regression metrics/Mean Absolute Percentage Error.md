**Mean Absolute Percentage Error (MAPE)** is a [[metric]] measures the ratios of the absolute error to the actual value. MAPE is a **Loss function**, corresponding to the expected value of the squared error loss.

#### Evaluation Function:
$$
MAPE = \frac{1}{n} \sum_{i=1}^n \frac{|y_i - \hat y_i|}{|y_i|}
$$

#### Derivative of a Function:
$$
\delta MAPE = \frac{1}{n} \sum_{i=1}^n \frac{sgn(\hat y_i - y_i)}{|y_i|}
$$

#### Pros and Cons:

* Pros:
	* Intuitive handling of input data
	* Scale-invariant (MAPE is scale-invariant, which means that it's not affected by the scale of the target variable. This can be an advantage when dealing with data that has widely varying scales)
* Cons:
	* Undefined for zero values ($y_i \neq 0$)
	* Sensitive to outliers (with a small amount of data the error increases greatly)
	* Not differentiable at 0
	* Does not account for bias (like MSE, MAPE measures the average difference between the predicted and actual values, but it doesn't account for bias in the model)