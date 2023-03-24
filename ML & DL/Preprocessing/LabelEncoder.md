**LabelEncoder** is a [[preprocessing]] method for encoding categorical variables into numerical values, which can be used as input for ML [[model]]. In other words, it's a process of converting categorical data into a numerical form, so that the algorithm can understand and operate on it / [source](https://github.com/Djacon/skmini/blob/main/skmini/preprocessing/_label.py#L6)

#### Example:

```python
>>> from sklearn import preprocessing
>>> le = preprocessing.LabelEncoder()
>>> le.fit([1, 2, 2, 6])
LabelEncoder()
>>> le.classes_
array([1, 2, 6])
>>> le.transform([1, 1, 2, 6])
array([0, 0, 1, 2])
>>> le.inverse_transform([0, 0, 1, 2])
array([1, 1, 2, 6])
```