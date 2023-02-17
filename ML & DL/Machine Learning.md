**Machine Learning (ML)** is a field of inquiry devoted to understanding and building methods that 'learn', that is, methods that leverage [[data]] to improve performance on some set of tasks. It's seen as part of [[Artificial Intelligence]] (AI)

Machine learning approaches are traditionally divided into three broad categories, which correspond to learning paradigms, depending on the nature of the "signal" or "feedback" available to the learning system:

#### The main fields of Machine Leaning:

* [[Supervised learning]] (SL)
	* [[Classification]]
		* $Y = \{0,\ 1\}^n$
	* [[Regression]]
		* $Y = \mathbb{R}$
* [[Unsupervied learning]]
	* Clustering
	* Dimensionalty Reduction
* [[Reinforcement learning]] (RL)


![[ML_image.jpg]]


# 2. Supervised Learning
## 2.1. Linear model

**Linear models** is a models in the form:
$$  
y = w_0 + w_1x_1 + w_2x_2 +... + w_nx_n = w_0 + \sum_{i=1}^nw_ix_i
$$
$$
y = \braket{x, w} + w_0
$$

****

### Gradient Descent  
$$  
w_j \rightarrow w_j - \alpha \cdot \frac{\delta L}{\delta w_j}  
$$  
  
**Time Complexity**:  
  
- $O(NDS)$, where N - sample size, D - number of features  
  
**Space Complexity**:  
  
- $O(ND)$