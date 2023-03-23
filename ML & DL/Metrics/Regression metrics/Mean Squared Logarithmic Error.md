**Mean Squared Logarithmic Error (MSLE)** is a commonly used [[metric]] and loss function in regression tasks, which measures the difference between the logarithm of predicted values and the logarithm of actual values

#### Evaluation Function:
$$
MSLE = \frac{1}{n} \sum_{i=1}^n (\ln(1 + y_i) - \ln(1 + \hat y_i))^2
$$

#### Derivative of a Function:
$$
\delta MSLE = \frac{2}{n} \sum_{i=1}^n (\ln(1 + \hat y_i) - \ln(1 + y_i))\cdot\frac{1}{1+\hat y_i}
$$

#### Pros and Cons:

* Pros:
	* Useful when the target variable has a wide range of values
	* Penalizes large differences between predicted and actual values more heavily than smaller differences
	* Less sensitive to outliers than MSE (thanks to logarithmic scale)
* Cons:
	* Cannot handle negative values (due to logarithm)
	* As with other loss functions, MSLE may not always be the most appropriate choice for a given task and other options may need to be explored