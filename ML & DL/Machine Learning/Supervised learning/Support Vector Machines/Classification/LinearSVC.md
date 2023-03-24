**LinearSVC** is a linear version of [[support vector classification]] (SVC), which is a popular machine learning algorithm used for binary [[classification]]. LinearSVC works by finding the best hyperplane that can separate data points of different classes with maximum margin / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_classification.py#L46)

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

# Get gradients of the loss function (Hinge / Squared Hinge)
Y_grad = _get_gradient_loss(y, y_pred)

# Update weights and bias
w -= learning_rate * Y_grad @ X / n

# Update with penalty (l1 / l2 / None)
w -= learning_rate * regularization(w)

b -= learning_rate * Y_grad.mean()
```