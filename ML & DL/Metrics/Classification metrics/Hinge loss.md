**Hinge loss** is a [[metric]] used for training classifiers. The hinge loss is used for "maximum-margin" classification, most notably for [[support vector machines]] (SVM)


#### Evaluation Function:
$$
HINGE = \begin{cases} 0, & \mbox{if } 1-y\cdot\hat y \leq 0\\1-y\cdot\hat y, & \mbox{otherwise} \end{cases}
$$

#### Derivative of a Function:
$$
\delta HINGE = \begin{cases} 0, & \mbox{if } 1-y\cdot\hat y \leq 0 \\ -y, & \mbox{otherwise} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* Robust to outliers
	* Encourages sparsity (good for large number of features)
	* Seeks to maximize the margin between positive and negative examples
* Cons:
	* Binary classification only
	* Sensitive to scaling