**Regression** in probability theory and math [[statistics]] is a one-way stochastic relationship that establishes a relationship between random variables, that is, a math expression that reflects the relationship between the dependent variable $y$ and the independent variables $x$, provided that this expression will have statistical significance.

#### List of the main regression algorithms in ML:

1. [[Linear Regression]]
2. [[Ridge]] (L2-regularization)
3. [[Lasso]] (L1-regularization)
4. Decision Tree Regression
5. Random Forest Regressor
6. KNN
7. Support Vector Regression (SVR)
8. Gaussian Regression
9. Polynomial Regression


#### List of basic [[Metric]] for Regression:

1. [[Mean Squared Error]] (MSE)
	1. $MSE = \frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2$
2.  [[Mean Absolute Error]] (MAE)
	1. $MAE = \frac{1}{n} \sum_{i=1}^n |y_i - \hat y_i|$
3. [[Root Mean Squared Error]] (RMSE)
	1. $RMSE = \sqrt{\frac{1}{n} \sum_{i=1}^n (y_i - \hat y_i)^2}$
4. [[Mean Absolute Percentage Error]] (MAPE)
	1. $MAPE = \frac{1}{n} \sum_{i=1}^n \frac{|y_i - \hat y_i|}{|y_i|}$
5. [[R-Squared]] (Coefficient of determination)
	1. $R^2 = 1 - \frac{RSS}{TSS}$
6. [[Adjusted R-Squared]]
	1. $R^2_{adj} = 1 - \frac{(1-R^2)(n-1)}{(n-k-1)}$