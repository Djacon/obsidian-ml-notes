**GaussianNB** is a [[naive bayes]] algorithm used for [[classification]]. Its based on Bayes' theorem and assumes that the features in a dataset are independent of each other, given the class variable. The main advantage of GNB is its ability to handle high-dimensional data with many features

#### Probability formula:
$$
p(C_k\ |\ x_1,\ \dots,\ x_2) \propto p(C_k)\prod_{i=1}^np(x_i\ |\ C_k)
$$

#### Likelihood formula
$$
p(x_i\ |\ C_k) = \frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{1}{2}(\frac{x-\mu}{\sigma})^2}
$$