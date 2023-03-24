**MinMaxScaler** is a [[data normalization]] technique used in [[machine learning]] and data science to scale numerical data in a specific range. In MinMaxScaler, each feature is scaled to a given range, typically between 0 and 1 / [source](https://github.com/Djacon/skmini/blob/main/skmini/preprocessing/_data.py#L4)

#### Normalization Formula:
$$
X_{norm} = \frac{X - X_{min}}{X_{max} - X_{min}}
$$

#### Example:
```python
>>> from sklearn.preprocessing import MinMaxScaler
>>> data = [[-1, 2], [-0.5, 6], [0, 10], [1, 18]]
>>> scaler = MinMaxScaler()
>>> print(scaler.fit(data))
MinMaxScaler()
>>> print(scaler.data_max_)
[ 1. 18.]
>>> print(scaler.transform(data))
[[0.   0.  ]
 [0.25 0.25]
 [0.5  0.5 ]
 [1.   1.  ]]
>>> print(scaler.transform([[2, 2]]))
[[1.5 0. ]]
```