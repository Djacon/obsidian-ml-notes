**Manhattan normalization (or Taxicab norm, $l_1$-distance)** is a [[distance metric]] whose usual distance function or metric of Euclidean geometry is replaced by a new metric in which the distance between two points is the sum of the absolute differences of their Cartesian coordinates

#### Evaluation Function:
$$
||x||_1 := \sum_{i=1}^n|x_i|
$$

#### Derivative of a Function:
$$
\delta ||x||_1 = \sum_{i=1}^nsgn(x_i)
$$

#### Pros and Cons:

* Pros:
	* Helps eliminate the problem of scale differences in feature vectors
	* Robust to outliers (unlike Euclidean norm, which can amplify noise or outliers, Manhattan norm is less sensitive to extreme values and can be more robust to outliers)
	* May be more appropriate for some applications because it can reflect sparsity and data structure
* Cons:
	* May not preserve the direction of the feature vector, unlike Euclidean normalization
	* Can lead to loss of information especially when the length of the vector is small (this is because the normalization reduces the magnitudes of the features and can lead to loss of discriminative power in some cases)
	* May not be suitable for all algorithms (some algorithms, such as KNN, may perform better with Euclidean norm, as they rely on the distance between feature vectors, which is better to compute using Euclidean distance)