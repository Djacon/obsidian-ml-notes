**RMSProp (Root Mean Square Propagation)** is a [[optimization algorithm]] that adapts the learning rate for each parameter based on the root mean squared [[gradient|gradients]] of the previous time steps. The main idea behind RMSProp is to reduce the learning rate for parameters that have high variance in the gradients, while increasing the learning rate for parameters that have low variance in the gradients

#### Optimization Algorithm:
$$
v_{\delta w_j} \leftarrow \beta \cdot v_{\delta w_j} + (1 - \beta) \cdot \delta w_j^2
$$
$$
w_j \leftarrow w_j - \alpha\cdot \frac{\delta w_j}{\sqrt{v_{\delta w_j}} + \epsilon},
$$

#### Pros and Cons:

* Pros:
	* Adaptive to learning rate
	* Can handle non-stationary objectives and noisy gradients
	* Only two hyperparameters (learning rate $\alpha$ and decay rate $\beta$)
* Cons:
	* Sensitive to hyperparameters
	* Large memory usage (bad for large datasets)
	* In some cases can overshoot the local minima

#### Addition:

* **Time Complexity**:
	- -
- **Space Complexity**: 
	- -