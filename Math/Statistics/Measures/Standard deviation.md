**Standard deviation (std, or $\sigma$)** is a measure that find the dispersion of a dataset relative to its mean. The standard deviation is calculated as the square root of [[variance]] by determining each data point's deviation relative to the [[mean]]

#### Math formula:
$$
\sigma = \sqrt\frac{\sum (x_i - \bar x)^2}{n - 1},\ \sigma = \sqrt{D}
$$

#### Function implementation:

```python
# Numpy implementation
std = np.std(sample, ddof=1)

# Build-in method
x_mean = sum(sample) / len(sample)
std = (sum((x - x_mean) ** 2 for x in sample) / (len(sample) - 1)) ** .5
```


##### Variance properties:
* $D_{x+C} = D_x$
* $std_{x+C} = std_x$

* $D_{x\cdot C} = D_x \cdot C^2$
* $std_{x\cdot C} = std_x \cdot C$