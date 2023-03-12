**Adam (ADAptive Moment estimator)** is an [[optimization algorithm]] that combines the benefits of both [[RMSProp]] and momentum optimization. It maintains a moving average of the gradients and their squared values and uses them to adapt the learning rate of each weight during training.

#### Optimization Algorithm:
$$
m_{\delta w_j} \rightarrow \frac{\beta_1 \cdot m_{\delta w_j} + (1 - \beta_1) \cdot \delta w_j}{1 - \beta_1^t}
$$
$$
v_{\delta w_j} \rightarrow \frac{\beta_2 \cdot v_{\delta w_j} + (1 - \beta_2) \cdot \delta w_j^2}{1 - \beta_2^t}
$$
$$
w_j \rightarrow w_j - \alpha\cdot \frac{m_{\delta w_j}}{\sqrt{v_{\delta w_j}} + \epsilon},
$$

#### Pros and Cons:

* Pros:
	* Fast convergence and improved performance on a large datasets
	* Resistant to getting stuck in local minima and saddle points
	* Only three hyperparameters (learning rate $\alpha$ and two decay rate $\beta_1$ and $\beta_2$)
* Cons:
	* Sensitive to hyperparameters
	* Large memory usage (bad for large datasets)
	* In some cases can converge to a suboptimal solution

#### Addition:

* **Time Complexity**:
	- -
- **Space Complexity**: 
	- -