**Linear Regression (LR)** is a statistical [[supervised learning]] linear model to predict the quantitative variable by forming a linear relationship with one or more independent features by minimazing the [[Residual Sum of Squares]] (RSS)

#### Loss Function:
$$
Loss = RSS = \sum_{i=1}^n(y_i-\hat y_i)^2
$$

#### Derivative of a Function:
$$
\delta Loss = \delta RSS = 2\sum_{i=1}^n(\hat y_i-y_i)
$$

#### Analytic Solution:
$$
w = (X^TX)^{-1}X^Ty
$$

#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function
Y_grad = _get_gradient_loss(y, y_pred) # ex: Y = 2 * (y_pred - y)

# Update weights and bias
w -= learning_rate * Y_grad @ X
b -= learning_rate * Y_grad.sum()
```