**Root Mean Squared Error (RMSE)** is a [[metric]] measured the root of the [[mean squared error]] - that is, the root of the average squared difference between the estimated values and the actual value. RMSE is a **Loss function**, corresponding to the expected value of the squared error loss.

#### Evaluation Function:
$$
RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2} = \sqrt{MSE}
$$

#### Derivative of a Function:
$$
\delta RMSE = \frac{\sum_{i=1}^n (\hat y_i - y_i)}{\sqrt{n\sum_{i=1}^n (y_i - \hat y_i)^2}} = \frac{\delta MSE}{2\sqrt{MSE}}
$$

#### Pros and Cons:

* Pros:
	* Intuitive handling of input data
	* Sensitivity to outliers (that's a big plus when we need to punish heavily for big errors)
	* Differentiability
	* Units of measurement (like MAE, RMSE has the same units as the target variable, which makes it easy to interpret the value of RMSE in real-world terms)
	* Commonly used (RMSE is a very commonly used metric in machine learning, which means that it's easy to find examples of its use)
* Cons:
	* Not robust to outliers (that's a big disadvantage when we have a lot of outliers in the data)
	* Does not account for variance: (if the predictions are scattered above and below the actual values they can have good MSE accuracy, while the model does poorly)
	* Magnifies errors (because RMSE takes the square root of the average of the squared differences between the predicted and actual values, it magnifies errors, especially for large errors)