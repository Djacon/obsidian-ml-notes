**Stochastic Gradient Descent (SGD)** is a popular [[optimization algorithm]] used in ML and DL for minimizing the loss function during the training of a model. It's an iterative method that updates the parameters of the model based on the gradients of a small subset of the training data (batch)

#### Optimization Algorithm:
$$ 
w_j \rightarrow w_j - \frac{\alpha}n \sum_{i=1}^n\frac{\delta L_i}{\delta w_j}  
$$

#### Addition:

* **Time Complexity**:
	- $O(NDS)$, where N - batch size, D - number of features  
- **Space Complexity**: 
	- $O(ND)$