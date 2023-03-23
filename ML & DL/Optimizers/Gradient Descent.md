**Gradient descent** is a first-order iterative [[optimization algorithm]] used to minimize a given function, such as a loss function in ML. The goal is to find the minimum value of the function by iteratively moving towards its local or global minimum

#### Optimization Algorithm:
$$
w_j \leftarrow w_j - \alpha \cdot \delta w_j
$$

#### Pros and Cons:

* Pros:
	* Converges (gradient descent is guaranteed to converge to a minimum of a function)
	* Simplicity (easy to understand and implement)
	* Good for small datasets
* Cons:
	* Computationaly expensive for large datasets (it compute gradient of all data every iteration)
	* Highly dependent to hyperparameters (such as learning rate - $\alpha$)
	* Tendency to local optima

#### Addition:

* **Time Complexity**:
	- -
- **Space Complexity**: 
	- -