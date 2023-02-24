**Variance (Дисперсия)** is the expectation of the squared deviation of a random variable from its population mean or sample mean. Variance is a measure of dispersion, meaning it is a measure of how far a set of numbers is spread out from their average value

#### Math formula:
$$
D = \frac{\sum (x_i - \bar x)^2}{n - 1},\ \sqrt{D}=\sigma \ (std)
$$

#### Function implementation:

```python
# Numpy implementation
D = np.var(sample, ddof=1)

# Build-in method
x_mean = sum(sample) / len(sample)
D = sum((x - x_mean) ** 2 for x in sample) / (len(sample) - 1)
```


##### Variance properties:
* $D_{x+C} = D_x$
* $std_{x+C} = std_x$

* $D_{x\cdot C} = D_x \cdot C^2$
* $std_{x\cdot C} = std_x \cdot C$