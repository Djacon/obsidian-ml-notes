**SGDRegressor** is a statistical [[supervised learning]] linear model to predict the quantitative variable by forming a linear relationship with one or more independent features by using the [[Stochastic Gradient Descent]] (SGD)

#### Loss Function:
$$
Loss = \frac{1}{2n}RSS + r(w)
$$

#### Derivative of a Function:
$$
\frac{\delta Loss}{\delta w_j} = \frac{1}{n}\sum_{i=1}^n(\hat y_i-y_i)\cdot x_{ji} + \frac{\delta r(w_j)}{\delta w_j}
$$

#### Analytic Solution:
<h5 align='center' style='color:red'>There is no closed-form solution</h5>
#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function
Y_grad = _get_gradient_loss(y, y_pred) # ex: Y = 2 * (y_pred - y)

# Update weights and bias
w -= learning_rate * Y_grad @ X / (2 * n)

# Update with penalty (l1 / l2 / elastic-net / None)
w -= learning_rate * regularization(w)

b -= learning_rate * Y_grad.mean()
```
