**Hidge loss** is a [[metric]] used for training classifiers. The hinge loss is used for "maximum-margin" classification, most notably for support vector machines (SVMs)


#### Evaluation Function:
$$
HIDGE = \begin{cases} 0, & \mbox{if } 1-y_i\cdot\hat y_i \leq 0 \\ 1-y_i\cdot\hat y_i, & \mbox{otherwise.} \end{cases}
$$

#### Derivative of a Function:
$$
\delta HIDGE = \begin{cases} 0, & \mbox{if } 1-y_i\cdot\hat y_i \leq 0 \\ -y_ix_i, & \mbox{otherwise.} \end{cases}
$$

#### Pros and Cons:

* Pros:
	* -
* Cons:
	* -