**Elastic net** is a [[Linear Regressor]] model is a regularized regression method that linearly combines the L1 and L2 penalties of the [[Lasso]] and [[Ridge]] methods. Also it used in the fitting of linear or logistic regression models

#### Cost Function:
$$
Cost = \frac{1}{2n}RSS + \lambda\cdot l^1_{ratio}\cdot ||w||_1 + \frac{\lambda}2 \cdot (1-l^1_{ratio}) \cdot ||w||^2_2
$$

#### Derivative of a Function:
$$
\frac{\delta Cost}{\delta w_j} = \frac{1}{n}\sum_{i=1}^n(\hat y_i-y_i)\cdot x_{ji} + \lambda\cdot (l^1_{ratio}\cdot sgn(w_j) + (1-l^1_{ratio})\cdot w_j)
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
w -= learning_rate * alpha * (l1_ratio * np.sign(w) + (1 - l1_ratio) * w)

b -= learning_rate * Y_grad.mean()
```