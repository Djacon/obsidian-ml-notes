**Residual Sum of Squares (RSS)** is also known as the **Sum of Squared estimate of Errors (SSE)**, is a [[metric]] measured the sum of the squares of residuals. A small RSS indicates a tight fit of the model to the data. It is used as an optimality criterion in parameter selection and model selection

#### Evaluation Function:
$$
RSS = \sum_{i=1}^n(y_i-\hat y_i)^2
$$

#### Derivative of a Function:
$$
\delta RSS = 2\sum_{i=1}^n (\hat y_i - y_i)
$$

#### Pros and Cons:

* Pros:
	* Intuitive handling of input data
	* Easy to differentiate
	* Commonly used (RSS is a very commonly used metric in machine learning, which means that it's easy to find examples of its use)
* Cons:
	* Units of measurement (RSS has no defined unit of measurement, which makes it difficult to interpret the metric value in real-world terms)
	* Does not account for variance: (if the predictions are scattered above and below the actual values they can have good RSS accuracy, while the model does poorly)