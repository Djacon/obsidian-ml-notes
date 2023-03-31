**Leaky ReLU** is a variation of the popular [[Rectified Linear Unit]] (ReLU) [[activation function]] that addresses one of the drawbacks of the original ReLU function. It's a simple function that returns the maximum of its input and other value $\alpha \in (0; 1)$

#### Activation Function:
$$
\mbox{Leaky ReLU}(z) = \max(\alpha x,\ x)
$$

#### Derivative of a Function:
$$
\mbox{Leaky ReLU}'(z) = \begin{cases} 1, & \mbox{if } z > 0\\\alpha, & \mbox{otherwise} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* Computationally efficient
	* Non-saturating
	* Solves the "dying ReLU" problem by allowing non-zero gradient
	* Sparsity (it can produce sparsity in activations, where many of the output values are zero)
* Cons:
	* Not fully zero-centered
	* Additional hyperparameter ($\alpha$)
	* Dying ReLU problem (neurons can die if they get stuck in the negative region, where the gradient is always zero)