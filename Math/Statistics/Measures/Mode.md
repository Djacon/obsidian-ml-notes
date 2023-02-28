**Mode** is a number that describes the most frequent value in the [[sample]]. If $X$ is a discrete random variable, the mode is the value $x$ at which the probability mass function takes its maximum value (i.e, $x=\arg\underset{x_i}\max P(X = x_i)$). In other words, it is the value that is *most likely* to be sampled

#### Math formula:
$$
M_x = \arg\underset{x_i}\max P(X = x_i)
$$

#### Function implementation:

```python
import statistics as stats

# Statistics implementation
M_x = stats.mode(sample)

# Build-in method
M_x = max(sample, key=sample.count)
```
