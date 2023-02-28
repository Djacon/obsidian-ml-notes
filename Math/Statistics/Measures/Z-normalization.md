**Z-normalization (Z-norm/Z-score)** is a measure that refers to the process of normalizing every value in a dataset such that the [[mean]] of all of the values is 0 ($M_z = 0$) and the [[standard deviation]] is 1 ($\sigma_z = 1$)

#### Math formula:
$$
Z = \frac{X-M_x}{\sigma_x} \ or\ Z_n = \frac{\bar X_n-M_x}{\sigma_x/\sqrt{n}}
$$


#### Function implementation:

```python
# Scipy.stats implementation
Z = scipy.stats.zscore(sample)

# Build-in method
x_mean = sum(sample) / len(sample)
std = (sum((x - x_mean) ** 2 for x in sample) / (len(sample) - 1)) ** .5
Z = [(x - x_mean) / std for x in sample]
```
