**Linear Regression (LR)** is a statistical [[supervised learning]] linear model to predict the quantitative variable by forming a linear relationship with one or more independent features by minimazing the [[Residual Sum of Squares]] (RSS)

#### Loss Function:
$$
Loss = RSS = \sum_{i=1}^n(y_i-\hat y_i)^2
$$

#### Derivative of a Function:
$$
\delta Loss = \delta RSS = 2\sum_{i=1}^n(\hat y_i-y_i)
$$

#### Solution Algorithm:
$$
w = (X^TX)^{-1}X^Ty
$$


#### Addition:

**Ordinary Least Squares (OLS)** is the simplest method for solving problems using linear regression

$$
|y - Xw|^2_2 \rightarrow \min_w
$$

**Time Complexity**: 
- $O(N^2D+D^3)$, where N - sample size, D - number of features  

**Space Complexity**:  
-  ¯\\_(ツ)_/¯ 