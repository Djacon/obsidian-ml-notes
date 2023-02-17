**Mean Absolute Error (MAE)** is a [[metric]] measured the average of the absolute errors - that is, the average absolute difference between the estimated values and the actual value. MAE is a **Loss function**, corresponding to the expected value of the squared error loss.

#### Evaluation Function:
$$
MAE = \frac{1}{n} \sum_{i=1}^n |y_i - \hat y_i|
$$

#### Derivative of a Function:
$$
\delta MAE = \frac{1}{n} \sum_{i=1}^n sgn(\hat y_i - y_i)
$$

#### Pros and Cons:

* Pros:
	* Intuitive handling of input data
	* Sensitivity to outliers (unlike MSE, it is more robust to outliers, which is an advantage when we have a lot of them)
	* Easy to differentiate
	* Units of measurement (unlike MSE, MAE has the same units as the target variable)
* Cons:
	* Less sensitive to differences
	* Does not account for bias (like MSE, MAE measures the average difference between the predicted and actual values, but it doesn't account for bias in the model)