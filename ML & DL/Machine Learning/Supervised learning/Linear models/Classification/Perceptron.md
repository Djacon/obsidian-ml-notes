**Perceptron** is a [[linear classifier]] which is used in binary [[classification]] problems. It is a simple and efficient algorithm for training a linear binary classifier. The algorithm uses [[Hinge loss]] and one of the three regularizers / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_classification.py#L72)

#### Cost Function:
$$
Cost = HINGE + r(w)
$$

#### Derivative of a Function:
$$
\frac{\delta Cost}{\delta w_j} = \frac{\delta HINGE}{\delta w_j} + \frac{\delta r(w_j)}{\delta w_j}
$$

#### Analytic Solution:
<h5 align='center' style='color:red'>There is no closed-form solution</h5>
#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function (Hinge)
Y_grad = _get_gradient_loss(y, y_pred) # ex: Y = 2 * (y_pred - y)

# Update weights and bias
w -= learning_rate * Y_grad @ X / n

# Update with penalty (l1 / l2 / elastic-net / None)
w -= learning_rate * regularization(w)

b -= learning_rate * Y_grad.mean()
```