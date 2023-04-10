**Hyperbolid Tangent (Tanh)**, in [[deep learning]], is a type of [[activation function]] commonly used in [[neural network|neural networks]]. It's a non-linear function that squashes any real-valued number to a value between -1 and 1

![[Tanh_image.png|400]]

#### Activation Function:
$$
\tanh(z) = \frac{e^z-e^{-z}}{e^z+e^{-z}}
$$

#### Derivative of a Function:
$$
\tanh'(z) = 1-\tanh^2(z) = \frac{4}{(e^z+e^{-z})^2}
$$

#### Pros and Cons:

* Pros:
	* Zero-centered
	* Symmetry function
	* It has smooth derivative
* Cons:
	* Problem of [[gradient decay]]
	* Computationally expensive
	* Prone to saturation