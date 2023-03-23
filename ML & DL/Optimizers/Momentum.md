**Momentum** is a [[optimization algorithm]] that used to speed up the convergence of the algorithm towards the minimum of the loss function. Momentum involves adding a fraction of the previous update to the current update during training of the machine learning model

#### Optimization Algorithm:
$$
m_{\delta w_j} \leftarrow \beta \cdot m_{\delta w_j} + (1 - \beta) \cdot \delta w_j
$$
$$
w_j \leftarrow w_j - \alpha\cdot \frac{\delta w_j}{\sqrt{m_{\delta w_j}} + \epsilon},
$$

#### Pros and Cons:

* Pros:
	* Fast convergence and improved performance on a large datasets
	* Resistant to getting stuck in local minima and saddle points
	* Particularly effective in cases where the gradient of the loss function is noisy
* Cons:
	* Sensitive to hyperparameters
	* When $\beta$ is set too high, then the algorithm can converge too quickly and result in a suboptimal solution
	* Difficult to visualize or intepret

#### Addition:

* **Time Complexity**:
	- -
- **Space Complexity**: 
	- -