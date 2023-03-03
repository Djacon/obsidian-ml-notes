**Linear Regressors** is a family of models that are a linear combination of $w$ weights, $\phi(x)$ nonlinear functions and independent variables $X$. It's usually used when solving [[regression]] problems, but can also be used when working with time series analysis

#### Prediction formula:
$$
y = w_0 + w_1x_1 +\ \dots\ + w_nx_n + \epsilon = w\cdot x + \epsilon
$$

![[LR_image.png]]

**When we work with a simple linear model, we can write the linear function as follows:**
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