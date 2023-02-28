**HuberRegressor** is a statistical [[supervised learning]] linear model to predict the quantitative variable by forming a linear relationship with one or more independent features by using the [[Huber loss]] and [[Euclidean distance]]

#### Loss Function:
$$
Loss = HUBER + \lambda\cdot||w||^2_2
$$


#### Derivative of a Function:
$$
\frac{\delta Loss}{\delta w_j} = \frac{\delta HUBER}{\delta w_j} + 2\lambda\cdot w_j
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
w -= learning_rate * (Y_grad @ X + 2 * alpha * w)
b -= learning_rate * Y_grad.sum()
```