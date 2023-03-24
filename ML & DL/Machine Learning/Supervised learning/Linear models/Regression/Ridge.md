**Ridge (L2-regularization)** is a [[linear regressor]] of estimating the coefficients of multiple-regression models in scenarios where the independent variables are highly correlated. Can be calculated by finding the [[Mean Squared Error]] (MSE) and [[Euclidean distance]] / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_regression.py#L29)

#### Cost Function:
$$
Cost = MSE + \lambda\cdot||w||^2_2 = \sum_{i=1}^n(y_i-\hat y_i)^2 + \lambda\sum_{j=1}^p w_j^2
$$

#### Derivative of a Function:
$$
\frac{\delta Cost}{\delta w_j} = \frac{\delta MSE}{\delta w_j} + 2\lambda\cdot w_j = 2\cdot\left(\sum_{i=1}^n(\hat y_i-y_i)\cdot x_{ji} + \lambda\cdot w_j\right)
$$

#### Analytic Solution:
$$
w = (X^TX+\lambda I)^{-1}X^Ty
$$

#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function
Y_grad = _get_gradient_loss(y, y_pred) # Y = 2 * (y_pred - y)

# Update weights and bias
w -= learning_rate * (Y_grad @ X / n + 2 * alpha * w)
b -= learning_rate * Y_grad.mean()
```