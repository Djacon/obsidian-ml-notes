**Logistic Regression** is a statistical [[linear classifier]] used to predict the probability of an event occurring by comparing it to a logistic curve. This regression gives the answer as the probability of a binary event (1 or 0) / [source](https://github.com/Djacon/skmini/blob/main/skmini/linear_model/_classification.py#L13)

#### Cost Function:
$$
Loss = -\frac{1}{n}\sum_{i=1}^n (y_i\log(\hat y_i)\ + (1-y_i)\log(1-\hat y_i)) + r(w)
$$

#### Derivative of a Function:
$$
\frac{\delta Loss}{\delta w_j} = \frac{1}{n}\sum_{i=1}^n \frac{\hat y_i - y_i}{\hat y_i\cdot(1 - \hat y_i)}\cdot x_{ji} + \frac{\delta r(w_j)}{\delta w_j}
$$

#### Numerical method:

```python
# Get predictions
y_pred = X @ w + b

# Get gradients of the loss function
Y_grad = _get_gradient_loss(y, y_pred)

# Update weights and bias
w -= learning_rate * Y_grad @ X / n

# Update with penalty (l1 / l2 / elastic-net / None)
w -= learning_rate * regularization(w)

b -= learning_rate * Y_grad.mean()
```

![[LogReg_image.webp]]