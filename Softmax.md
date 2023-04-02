**Softmax function** is a [[activation function]] that turns numbers aka logits into probabilities that sum to one. Softmax function outputs a vector that represents the probability distributions of a list of potential outcomes

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
	* 
* Cons:
	* 