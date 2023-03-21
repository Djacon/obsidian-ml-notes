**SGDRegressor** is a statistical supervised learning [[Linear Regressor]] to predict the quantitative variable by forming a linear relationship with one or more independent features by using the [[Stochastic Gradient Descent]] (SGD)

#### Cost Function:
$$
Cost = Loss + r(w)
$$ 
#### Derivative of a Function:
$$
\frac{\delta Cost}{\delta w_j} = \frac{\delta Loss}{\delta w_j} + \frac{\delta r(w_j)}{\delta w_j}
$$

#### Analytic Solution:
<h5 align='center' style='color:red'>There is no closed-form solution</h5>
#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function (MSE / Huber / etc..)
Y_grad = _get_gradient_loss(y, y_pred) # ex: Y = 2 * (y_pred - y)

# Update weights and bias
w -= learning_rate * Y_grad @ X / n

# Update with penalty (l1 / l2 / elastic-net / None)
w -= learning_rate * regularization(w)

b -= learning_rate * Y_grad.mean()
```
