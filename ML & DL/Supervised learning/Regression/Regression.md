**Regression** in probability theory and math [[statistics]] is a math expression that reflects the relationship between the dependent variable "$y$" and the independent variables $X$, provided that this expression will have statistical significance

#### List of the main regression algorithms in ML:

1. [[Linear Regression]]
2. [[Ridge]] (L2-regularization)
3. [[Lasso]] (L1-regularization)
4. Decision Tree Regression
5. Random Forest Regressor
6. K-Nearest Neighbours (kNN)
7. Support Vector Regression (SVR)
8. Gaussian Regression
9. Polynomial Regression


#### List of basic [[Metric]] for Regression:

1. [[Mean Squared Error]] (MSE)
	* $MSE = \frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2$
2.  [[Mean Absolute Error]] (MAE)
	* $MAE = \frac{1}{n} \sum_{i=1}^n |y_i - \hat y_i|$
3. [[Root Mean Squared Error]] (RMSE)
	* $RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2}$
4. [[Mean Absolute Percentage Error]] (MAPE)
	* $MAPE = \frac{1}{n} \sum_{i=1}^n \frac{|y_i - \hat y_i|}{|y_i|}$
5. [[R-Squared]] (Coefficient of determination)
	* $R^2 = 1 - \frac{RSS}{TSS}$
6. [[Adjusted R-Squared]]
	* $R^2_{adj} = 1 - \frac{(1-R^2)(n-1)}{(n-k-1)}$