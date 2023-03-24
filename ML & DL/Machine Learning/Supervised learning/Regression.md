**Regression** in probability theory and math [[statistics]] is a math expression that reflects the relationship between the dependent variable "$y$" and the independent variables $X$, provided that this expression will have statistical significance

#### List of the main regression algorithms in ML:

* [[Linear Regression]]
* [[Ridge]] (L2-regularization)
* [[Lasso]] (L1-regularization)
* [[DecisionTreeRegressor]]
* [[RandomForestRegressor]]
* [[KNeighborsRegressor]]
* [[Support Vector Regressor]] (SVR)


#### List of basic [[Metric]] for Regression:

* [[Mean Squared Error]] (MSE)
	* $MSE = \frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2$
* [[Mean Absolute Error]] (MAE)
	* $MAE = \frac{1}{n} \sum_{i=1}^n |y_i - \hat y_i|$
* [[Root Mean Squared Error]] (RMSE)
	* $RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2}$
* [[Mean Absolute Percentage Error]] (MAPE)
	* $MAPE = \frac{1}{n} \sum_{i=1}^n \frac{|y_i - \hat y_i|}{|y_i|}$
* [[R-Squared]] (Coefficient of determination)
	* $R^2 = 1 - \frac{RSS}{TSS}$
* [[Adjusted R-Squared]]
	* $R^2_{adj} = 1 - \frac{(1-R^2)(n-1)}{(n-k-1)}$