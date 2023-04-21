**Stochastic Gradient Descent (SGD)** is a popular [[optimization algorithm]] used in ML and DL for minimizing the loss function during the training of a model. It's an iterative method that updates the parameters of the model based on the [[gradient|gradients]] of a small subset of the training data (batch)

#### Optimization Algorithm:
$$ 
w_j \leftarrow w_j - \frac{\alpha}n \sum_{i=1}^n\delta w_j  
$$

#### Pros and Cons:

* Pros:
	* Computational efficiency (unlike [[gradient descent]], it computes only small subsets)
	* Memory efficiency (since only small subsets are computed, the computer uses less memory)
	* Good for large datasets
	* Robustness when dealing with noisy or sparse data
* Cons:
	* Slow convergence
	* Highly dependent to hyperparameters (such as learning rate - $\alpha$)
	* Tendency to local optima

#### Addition:

* **Time Complexity**:
	- -
- **Space Complexity**: 
	-  -