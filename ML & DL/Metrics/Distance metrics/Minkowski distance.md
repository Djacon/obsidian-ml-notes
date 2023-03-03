**Minkowski distance** is a [[distance metric]] in a normed vector space which can be considered as a generalization of both the [[Euclidean distance]] and the [[Manhattan distance]]. It is named after the German mathematician Hermann Minkowski

#### Evaluation Function:
$$
||x||_p := \left(\sum_{i=1}^n|x_i|^p \right)^{1/p}
$$

#### Derivative of a Function:
$$
\delta ||x||_p = \frac{\sum_{i=1}^n (x_i\cdot|x_i|^{p-2})}{\left({\sum_{i=1}^n|x_i|^p}\right)^{\frac{p-1}{p}}}
$$

#### Pros and Cons:

* Pros:
	* Helps to reduce the impact of outliers by using the square root
	* Can improve the performance of some algorithms like KNN or SVM
	* Maintains the direction of the feature vector (unlike Min-Max norm, which can change the direction of the feature vector, Euclidean norm maintains the direction of the vector, which can be useful for some applications.
* Cons:
	* Can amplify noise
	* May not be appropriate for all applications (this normalization assumes that all features are equally important and should be normalized in the same way)
	* Can lead to loss of information especially when the length of the vector is small (this is because the normalization reduces the magnitudes of the features and can lead to loss of discriminative power in some cases)