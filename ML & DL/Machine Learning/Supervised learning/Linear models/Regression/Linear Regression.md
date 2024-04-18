**Linear Regression (LR)** is a statistical [[supervised learning]] [[linear regressor]] to predict the continuous target variable by forming a linear relationship with one or more independent features by minimazing the [[Residual Sum of Squares]] (RSS) or [[Mean Squared Error]] (MSE) / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_regression.py#L11)

#### Cost Function:
$$
MSE = \frac{1}{n}\sum_{i=1}^n(y_i-\hat y_i)^2
$$

#### Derivative of a Function:
$$
\frac{\delta MSE}{\delta w_j} = \frac{2}{n}\sum_{i=1}^n(\hat y_i-y_i)x_{ji}
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
w -= learning_rate * Y_grad @ X / n
b -= learning_rate * Y_grad.mean()
```