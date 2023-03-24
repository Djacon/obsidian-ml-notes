**StandardScaler** is a [[data standardization]] technique that used [[z-normalization]] to transform the features of a dataset so that they have zero [[mean]] and unit [[variance]]


#### Normalization Formula:
$$
Z_{norm} = \frac{X - \mu}{\sigma} = \frac{X-X_{mean}}{X_{std}}
$$

#### Example:
```python
>>> from sklearn.preprocessing import StandardScaler
>>> data = [[0, 0], [0, 0], [1, 1], [1, 1]]
>>> scaler = StandardScaler()
>>> print(scaler.fit(data))
StandardScaler()
>>> print(scaler.mean_)
[0.5 0.5]
>>> print(scaler.transform(data))
[[-1. -1.]
 [-1. -1.]
 [ 1.  1.]
 [ 1.  1.]]
>>> print(scaler.transform([[2, 2]]))
[[3. 3.]]
```