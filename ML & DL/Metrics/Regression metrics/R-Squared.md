**$R^2$ (Coefficient of determination)** is a [[metric]] measures the share of variance of the dependent variable explained by the dependence model in question, i.e. by the explanatory variables. More precisely, it is one minus the share of unexplained variance in the variance of dependent variable

#### Evaluation Function:
$$
R^2 = 1 - \frac{RSS}{TSS} = 1 - \frac{\sum_{i=1}^n(y_i-\hat y_i)^2}{\sum_{i=1}^n(y_i-\bar y_i)^2}
$$

#### Derivative of a Function:
<h5 align='center' style='color:red'>Loss function is not implemented</h5>

#### Pros and Cons:

* Pros:
	* Intuitive handling of input data
	* Scale-invariant ($R^2$ is scale-invariant, which means that it's not affected by the scale of the target variable. This can be an advantage when dealing with data that has widely varying scales)
	* Useful for feature selection ($R^2$ can be used to evaluate the importance of the independent variables in the model. Variables with higher R-squared values are more important and should be retained in the model, while variables with lower $R^2$ values can be dropped)
* Cons:
	* Limited to linear models ($R^2$ is limited to linear models and may not be appropriate for non-linear models)
	* Doesn't provide information on the goodness of predictions ($R^2$ doesn't provide information on the accuracy of the predictions made by the model. A model with a high $R^2$ value can still make inaccurate predictions)