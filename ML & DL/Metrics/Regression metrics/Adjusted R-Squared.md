**$R^2_{adj}$ (Adjusted $R^2$)** an improved version of the [[R-squared]] [[metric]], which does not depend on the number of regressors (factors) and makes an adjustment for the number of independent variables in the model

#### Evaluation Function:
$$
R^2_{adj} = 1 - \frac{(1-R^2)(n-1)}{(n-k-1)}
$$

#### Derivative of a Function:
<h5 align='center' style='color:red'>Loss function is not implemented</h5>

#### Pros and Cons:

* Pros:
	* Penalty for unnecessary variables (Adjusted $R^2$ penalizes models that include unnecessary variables by adjusting $R^2$ value based on the number of variables in the model. This helps to prevent overfitting and ensures that the model is not including variables that do not improve its predictive power.
	* Useful for feature selection ($R^2$ can be used to evaluate the importance of the independent variables in the model. Variables with higher R-squared values are more important and should be retained in the model, while variables with lower $R^2$ values can be dropped)
	* More conservative than $R^2$ (Adjusted $R^2$ is more conservative than $R^2$, meaning that it is less likely to overestimate the predictive power of the model)
* Cons:
	* Limited to linear models ($R^2$ is limited to linear models and may not be appropriate for non-linear models)
	* More complex than $R^2$ (can be more difficult to interpret)
	* Assumes equal importance of variables (Adjusted $R^2$ assumes that all variables in the model are equally important, which may not be the case in practice)