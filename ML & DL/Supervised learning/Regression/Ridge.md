**Ridge (L2-regularization)** is a linear method of estimating the coefficients of multiple-regression models in scenarios where the independent variables are highly correlated. Can be calculated by finding the [[Residual Sum of Squares]] (RSS) and [[Euclidean normalization]]

#### Loss Function:
$$
Loss = RSS + \lambda\cdot||w||^2_2 = \sum_{i=1}^n(y_i-\hat y_i)^2 + \lambda\sum_{j=1}^p w_j^2
$$

#### Derivative of a Function:
$$
\delta Loss = \delta RSS + 2\lambda\cdot w = 2\cdot\left(\sum_{i=1}^n(\hat y_i-y_i) + \lambda\sum_{j=1}^p w_j\right)
$$

#### Solution Algorithm:
$$
w = (X^TX+\lambda I)^{-1}X^Ty
$$