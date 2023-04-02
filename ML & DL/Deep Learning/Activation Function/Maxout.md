**Maxout** is an [[activation function]] that is commonly used in [[deep learning]] [[neural networks]]. It was introduced as a way to overcome the limitations of other activation functions, such as the [[Rectified Linear Unit|ReLU]] and [[sigmoid]] functions, in certain types of neural networks

![[Maxout_image.png|300]]

#### Activation Function:
$$
\mbox{Maxout}(z) = \max(z_1,\ z_2)
$$

#### Derivative of a Function:
$$
\mbox{Maxout}'(z) = \begin{cases} (1,\ 0), & \mbox{if } z_1 > z_2\\(0,\ 1), & \mbox{otherwise} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* Flexibility (it can approximate any convex function)
	* Better performance in certaing cases (especally CNNs)
	* Prevent Overfitting (by adding multiple function for each feature)
* Cons:
	* Hard to interpret
	* Computationally expensive
	* Require more parameters

