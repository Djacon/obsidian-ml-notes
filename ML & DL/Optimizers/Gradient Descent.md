**Gradient descent** is a first-order iterative [[optimization algorithm]] used to minimize a given function, such as a loss function in ML. The goal is to find the minimum value of the function by iteratively moving towards its local or global minimum.

#### Optimization Algorithm:
$$  
w_j \rightarrow w_j - \alpha \cdot \frac{\delta L}{\delta w_j}  
$$

#### Addition:

* **Time Complexity**:
	- $O(NDS)$, where N - sample size, D - number of features  
- **Space Complexity**: 
	- $O(ND)$