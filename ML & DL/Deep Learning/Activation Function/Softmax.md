**Softmax** is a [[activation function]] used in [[machine learning]], specifically in the context of [[classification]] problems. The softmax function takes as input a vector of scores or logits and converts them into a probability [[distribution]] over a set of classes

#### Activation Function:
$$
\mbox{Softmax}(z) = \frac{e^{z_i}}{\sum_{i=1}^n e^{z_i}}
$$

#### Derivative of a Function:
$$
\mbox{Softmax}'(z) = \frac{e^{z_i}(\sum_{i=1}^n e^{z_i}-e^{z_i})}{(\sum_{i=1}^n e^{z_i})^2}
$$

#### Pros and Cons:

* Pros:
	* Probability interpretation
	* Differentiability
	* Input normalization
* Cons:
	* Sensitive to outliers (specifically in imbalance data)
	* Computational expensive