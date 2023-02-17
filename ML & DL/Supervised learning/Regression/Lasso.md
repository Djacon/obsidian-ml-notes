**Lasso (L1-regularization)** is an alternative to ridge for regularizing linear regression. Can be calculated by finding the [[Residual Sum of Squares]] (RSS) and [[Manhattan normalization]]


#### Loss Function:
$$
Loss = \frac{1}{2n}RSS + \lambda\cdot||w||_1 = \frac{1}{2n}\sum_{i=1}^n(y_i-\hat y_i)^2 + \lambda\sum_{j=1}^p |w_j|
$$

#### Derivative of a Function:
$$
\delta Loss = \frac{1}{2n}\delta RSS + \lambda\cdot sgn(w) = \frac{1}{n}\sum_{i=1}^n(\hat y_i-y_i) + \lambda\sum_{j=1}^p sgn(w_j)
$$

#### Solution Algorithm:
$$
w = (X^TX+n\cdot\lambda I)^{-1}X^Ty
$$