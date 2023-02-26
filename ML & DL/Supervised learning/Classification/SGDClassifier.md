**SGDClassifier** is a [[linear classifier]] that implements [[stochastic gradient descent]] (SGD) training for linear classifiers. It supports various loss functions for classification, including the [[hinge loss]] (for SVM-style classification), the logistic loss (for logistic regression), and the modified Huber loss

#### Loss Function:
$$
Loss = not\ found
$$

#### Derivative of a Function:
$$
\frac{\delta Loss}{\delta w_j} = not\ found
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
w -= learning_rate * Y_grad @ X
w -= learning_rate * alpha * (l1_ratio * np.sign(w) + (1 - l1_ratio) * w)

b -= learning_rate * Y_grad.mean()
```
