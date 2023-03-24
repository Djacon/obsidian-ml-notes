**HuberRegressor** is a statistical supervised learning [[Linear Regressor]] to predict the quantitative variable by forming a linear relationship with one or more independent features by using the [[Huber loss]] and [[Euclidean distance]] / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_regression.py#L59)

#### Cost Function:
$$
Cost = HUBER + \lambda\cdot||w||^2_2
$$


#### Derivative of a Function:
$$
\frac{\delta Cost}{\delta w_j} = \frac{\delta HUBER}{\delta w_j} + 2\lambda\cdot w_j
$$

#### Analytic Solution:
<h5 align='center' style='color:red'>There is no closed-form solution</h5>
#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function
Y_grad = _get_huber_loss(y, y_pred)

# Update weights and bias
w -= learning_rate * (Y_grad @ X / n + 2 * alpha * w)
b -= learning_rate * Y_grad.mean()
```
