**Linear Regressors** is a family of [[model|models]] that are a linear combination of $w$ weights, independent variables $X$, and errors $\epsilon$. It's usually used when solving [[regression]] problems, but can also be used when working with time series analysis / [source](https://github.com/Djacon/skmini/blob/113a1021714606b838b470e6c62bbc389005bf1c/skmini/linear_model/_base.py#L12)

#### Prediction formula:
$$
y = w_0 + w_1x_1 +\ \dots\ + w_nx_n + \epsilon = w\cdot x + \epsilon
$$

![[LR_image.png|600]]

**When we work with a simple linear model, we can write the linear function as follows:**
$$
y = Xw + \epsilon,\mbox{where}
$$
$$
y =
\begin{bmatrix}
y_1\\
y_2\\
\vdots\\
\ y_k\
\end{bmatrix},\
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