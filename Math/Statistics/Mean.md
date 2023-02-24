**Mean** is a number that describes the average value in the [[sample]]. Often denoted by a line at the top $\bar x$ or just $M_x$


#### Math formula:
$$
M_x = \frac{1}{n}\sum_{i=1}^n x_i
$$

#### Function implementation:

```python
# Numpy implementation
M_x = np.mean(sample)

# Build-in method
M_x = sum(sample) / len(sample)
```


##### Properties of the mean value:
* $M_{x + C} = M_x + C$ (When each value of the set is shifted, the average value will also be shifted by the same value)
* $M_{x \cdot C} = M_x \cdot C$
* $\sum_{i=0}^n (x_i - M_x) = 0$