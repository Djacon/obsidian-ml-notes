**Linear Regression (LR)** is a statistical [[supervised learning]] model to predict the quantitative variable by forming a linear relationship with one or more independent features by minimazing the [[Residual Sum of Squares]] (RSS)

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

![[LR_image.png]]

We can write the linear function as follows:
$$
y = Xw + \epsilon,\ where
$$
$$
y =
\begin{bmatrix}
y_1\\
y_2\\
\vdots\\
\ y_k\
\end{bmatrix},
\ \
\epsilon =
\begin{bmatrix}
\epsilon_1\\
\epsilon_2\\
\vdots\\
\ \epsilon_k\
\end{bmatrix}
$$

$$
X =
\begin{bmatrix}
\ 1 & x_{11} & \dots & x_{1n}\\  
\ 1 & x_{21} & \dots & x_{2n}\\
\vdots & \vdots & \ddots & \vdots\\
\ 1 & x_{k1} & \dots & x_{kn}\
\end{bmatrix},
\ \
w =
\begin{bmatrix}
w_0\\
w_1\\
w_2\\
\vdots\\
\ w_n\
\end{bmatrix}
$$