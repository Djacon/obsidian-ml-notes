**Euclidean distance** (or $l_2$-distance) is a [[distance metric]] which gives the ordinary distance from the origin to the point X consequence of the Pythagorean theorem. This operation may also be referred to as SRSS, which is an acronym for the Square Root of the Sum of Squares

#### Evaluation Function:
$$
||x||_2 := \sqrt{\sum_{i=1}^nx_i^2}
$$

#### Derivative of a Function:
$$
\delta ||x||_2 = \frac{\sum_{i=1}^n x_i}{\sqrt{\sum_{i=1}^nx_i^2}}
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