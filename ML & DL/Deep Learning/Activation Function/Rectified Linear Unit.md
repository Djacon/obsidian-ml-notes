**Rectified Linear Unit (ReLU)** in [[deep learning]], is a popular [[activation function]] commonly used in [[neural networks]] models. In simple terms, the ReLU function returns the input if it is positive, and returns 0 if the input is negative

![[ReLU_image.png|400]]

#### Activation Function:
$$
\mbox{ReLU}(z) = \max(0,\ x)
$$

#### Derivative of a Function:
$$
\mbox{ReLU}'(z) = \begin{cases} 1, & \mbox{if } z > 0\\0, & \mbox{otherwise} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* Easy to understand and interpret
	* Computationally efficient
	* Non-saturating
	* Sparsity (it can produce sparsity in activations, where many of the output values are zero)
* Cons:
	* Not zero-centered
	* Dying ReLU problem (neurons can die if they get stuck in the negative region, where the gradient is always zero)