**Mean Squared Error (MSE)** is a [[metric]] measured the average of the square errors - that is, the average squared difference between the estimated values and the actual value. MSE is a **Loss function**, corresponding to the expected value of the squared error loss

#### Evaluation Function:
$$
MSE = \frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2
$$

#### Derivative of a Function:
$$
\delta MSE = \frac{2}{n} \sum_{i=1}^n (\hat y_i - y_i)
$$

#### Pros and Cons:

* Pros:
	* Intuitive handling of input data
	* Sensitivity to outliers (that's a big plus when we need to punish heavily for big errors)
	* Easy to differentiate
	* Commonly used (MSE is a very commonly used metric in machine learning, which means that it's easy to find examples of its use)
* Cons:
	* Not robust to outliers (that's a big disadvantage when we have a lot of outliers in the data)
	* Units of measurement (MSE has no defined unit of measurement, which makes it difficult to interpret the metric value in real-world terms)
	* Does not account for variance: (if the predictions are scattered above and below the actual values they can have good MSE accuracy, while the model does poorly)