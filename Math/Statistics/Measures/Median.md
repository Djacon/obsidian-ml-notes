**Median** is the value separating the higher half from the lower half of a data [[sample]], a [[population]], or a probability distribution


#### Math formula:
$$
M_x = \begin{cases} x_{(n+1)/2}, & \mbox{if } n\mbox{ is odd} \\ (x_{(n+2)/2}+x_{n/2})/2, & \mbox{if } n\mbox{ is even} \end{cases}
$$

#### Function implementation:

```python
# Numpy implementation
M_x = np.median(sample)

# Build-in method (suppose that sample is ordered)

n = len(samples)
if n % 2 == 1:
	M_x = sample[n // 2]
else:
	M_x = (sample[n // 2] + sample[n // 2 - 1]) / 2
```