**Naive Bayes** is a [[classification]] algorithm based on Bayes' theorem. It is called "naive" because it assumes that the features of a data point are independent of each other, even though this assumption is often not true in reality

The basic idea of Naive Bayes is to calculate the probability of each class given a set of input features, and then select the class with the highest probability as the output classification. This is done by multiplying the prior probability of each class by the conditional probability of each feature given the class, and then normalizing the result

#### Prediction Formula
$$
\hat y = \underset{k\in\{1,\dots,K\}}{\operatorname{argmax}} p(C_k)\prod_{i=1}^np(x_i\ |\ C_k)
$$

![[NaiveBayes_image.png]]