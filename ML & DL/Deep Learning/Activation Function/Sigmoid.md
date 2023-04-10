**Sigmoid function**, in [[deep learning]], is a type of [[activation function]] commonly used in [[neural network|neural networks]]. The sigmoid function is a non-linear function that maps any real-valued number to a value between 0 and 1

![[Sigmoid_image.png|400]]

#### Activation Function:
$$
\sigma(z) = \frac{1}{1+e^{-z}}
$$

#### Derivative of a Function:
$$
\sigma'(z) = \sigma(z)\cdot(1-\sigma(z)) = \frac{e^{-z}}{(1+e^{-z})^2}
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