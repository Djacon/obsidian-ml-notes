Sigmoid-weighted Linear Unit (SiLU) is an [[activation function]], an improved version of [[sigmoid]], which solves the [[gradient decay]] and saturation effect problems. It's smooth, monotonically increasing, which allows the [[model]] to learn more efficiently and converge quickly

![[SiLU_image.png|300]]

#### Activation Function:
$$
\mbox{SiLU}(z) = \frac{z}{1+e^{-z}}
$$

#### Derivative of a Function:
$$
\mbox{SiLU}'(z) = \frac{e^z\cdot(z+e^z+1)}{(1+e^z)^2}
$$

#### Pros and Cons:

* Pros:
	* Easy to understand and interpret
	* Useful for binary classification
	* It has smooth derivative
* Cons:
	* Problem of [[gradient decay]]
	* Not zero-centered
	* Prone to saturation (this can lead to slow converges)