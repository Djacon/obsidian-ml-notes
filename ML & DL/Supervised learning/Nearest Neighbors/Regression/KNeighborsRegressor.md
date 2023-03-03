**KNeighborsRegressor** is a popular [[nearest neighbors]] algorithm for [[regression]] tasks. In KNN, the prediction of a new data point is based on the [[mean]] of its k nearest neighbors in the training dataset. The value of $k$ is a hyperparameter that needs to be set before training the algorithm

#### Distance metric:
$$
D = \left(\sum_{i=1}^n|x_i|^p \right)^{1/p}, \mbox{ default }p = 2
$$

#### Numerical method:

```python
from statistics import mean

# List of all predictions
y_pred = []

# Get prediction for each value
for x_test in X_test:
	# Get distance to each point (Euclidean / Manhattan / etc)
	dist = [distance(x_test, x_train) for x_train in X_train]
	
	# Get nearest k values
	labels = y_train[np.argsort(dist)[:self.k]]
	
	# Save prediction
	y_pred.append(mean(labels))
```