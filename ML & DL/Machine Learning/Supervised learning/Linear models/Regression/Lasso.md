**Least Absolute Shrinkage and Selection Operator (L1-regularization)** is an alternative to [[ridge]] for regularizing [[linear regressor]]. Can be calculated by finding the [[Residual Sum of Squares]] (RSS) and [[Manhattan distance]] / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_regression.py#L20)

#### Cost Function:
$$
Cost = \frac{1}{2n}RSS + \lambda\cdot||w||_1 = \frac{1}{2n}\sum_{i=1}^n(y_i-\hat y_i)^2 + \lambda\sum_{j=1}^p |w_j|
$$

#### Derivative of a Function:
$$
\frac{\delta Cost}{\delta w_j} = \frac{1}{2n}\cdot\frac{\delta RSS}{\delta w_j} + \lambda\cdot sgn(w_j) = \frac{1}{n}\sum_{i=1}^n(\hat y_i-y_i)\cdot x_{ji} + \lambda\cdot sgn(w_j)
$$

#### Analytic Solution:
<h5 align='center' style='color:red'>There is no closed-form solution</h5>
#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function
Y_grad = _get_gradient_loss(y, y_pred) # Y = 2 * (y_pred - y)

# Update weights and bias
w -= learning_rate * (Y_grad @ X / (2 * n) + alpha * np.sign(w))
b -= learning_rate * Y_grad.mean()
```
