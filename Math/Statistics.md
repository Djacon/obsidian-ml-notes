Statistics is a mathematical body of science that refers to the collection, analysis, interpretation or explanation, and presentation of [[data]], or as a branch of math. Some consider statistics to be a distinct mathematical science rather than a branch of mathematics. While many scientific investigations make use of data, statistics is concerned with the use of data in the context of uncertainty and decision making in the face of uncertainty.

## 1. Introduction:
### 1.1 Population and sample

The Population is the entire population of units of observation that are relevant to the topic of the study. For example, if you are doing a product study, your general population is likely to be all service users or a specific segment.

A sample population is the part of the population that you study using tools you've developed (questionnaire, guide, etc.).

**There are 3 types of Sampling:**
1. Simple random sample (We select random values from the whole sample)
2. Stratified sample (We divide the sample into some groups and take random values from each)
3. Cluster sample (We divide the sample into clusters, select only some of them, and take random values from there)

![[Sampling_image.png]]


### 1.2 Type of variables in statistics

1. Quantitative - measured values:
	1. Continuous (e.x.: $height \in (150, 200)$)
	2. Discrete (e.x.: 1, 2, 3, 4,...)
2. Nominative (categorical) - aggregated values (e.x. Male = 1; Female = 2)
3. Ordinal - operations of comparison


### 1.3 Central tendency measures

* **Mean** - average value in the sample
* **Median** - a number in the middle of an ordered dataset
* **Mode** - the most frequent value in the sample

![[Measure_of_central_tendency_image.jpg]]

**Properties of the mean value**:
- $M_x = \frac{1}{n}\sum x_i$
* $M_{x + C} = M_x + C$ (When each value of the set is shifted, the average value will also be shifted by the same value)
* $M_{x \cdot C} = M_x \cdot C$
* $\sum_{i=0}^n (x_i - M_x) = 0$


### 1.4 Measure of Variability

**Range** (Размах) is a difference of maximum and minimum values
$$R = X_{max} - X_{min}$$

**Variance** (Дисперсия) is the average square of the deviations of individual values of a feature from their mean value

$$D = \frac{\sum (x_i - \bar x)^2}{n - 1},\ \sqrt{D}=\sigma \ (std)$$
![[Empirical_rule_image.jpg]]

**Variance properties:**
* $D_{x+C} = D_x$
* $std_{x+C} = std_x$

* $D_{x\cdot C} = D_x \cdot C^2$
* $std_{x\cdot C} = std_x \cdot C$


### 1.5 Distribution quartiles and boxplot

**Quantile** is the value that a given random variable does not exceed with a fixed probability: $P(X \leq x_a) \geq \alpha$

**Quartiles** is a 3 points (feature values), which divides the ordered data set into 4 equal parts

**Boxplot** is a method that shows the distribution of quantitative data in a way that simplifies comparisons between variables or between levels of a categorical variable

![[Boxplot_outliers_image.webp]]

### 1.6 Normal Distribution

**Normal distribution** or **Gaussian distribution** is a type of continuous probability distribution for real-valued variable. The general form of its **probability density function** (PDF) is:

$$
f(x) = \frac{1}{\sigma\sqrt{2\pi}}e^{-(\frac{x-\mu}{4\sigma})^2}
$$

**Standardization (Z-normalization)** refers to the process of normalizing every value in a dataset such that the mean of all of the values is 0 ($M_z = 0$) and the standard deviation is 1 ($D_z = 1$)

$$
Z = \frac{X-\mu}\sigma \ or\ Z = \frac{\bar X-\mu}{\sigma/\sqrt{n}}
$$
Where:
-  **x**: Original value
-  **μ**: Mean of data
-  **σ**: Standard deviation of data
-  **n**: Number of samples

![[Standardized_normal_distribution_image.jpg]]


### 1.7 Central Limit Theorem

**The Central Limit Theorem (CLT)** establishes that, in many situations, for identically distributed independent samples, the standardized sample mean tends towards the standard normal distribution even if the original variables themselves are not normally distributed.

$$
Z = \lim_{n\rightarrow\infty}(\frac{X_n-\mu}{\sigma/\sqrt{n}})
$$

![[IllustrationCentralTheorem_image.jpg]]


### 1.8 Confidence intervals

The **Confidence Interval (CI)** is the range of values that you expect your estimate to fall between a certain percentage of the time if you run your experiment again or re-sample the population in the same way.

The **Standard Error (SE)** is the standard deviation (std) of its sampling distribution or an estimate of that standard deviation.

$$
\sigma_x^- = \frac{\sigma}{\sqrt{n}}\ or \ se = \frac{std}{\sqrt{n}}
$$

![[Confidence_interval_image.jpg]]


### 1.9 The idea behind statistical inference

**The null hypothesis ($H_0$)** is that there is **no significant** difference between the mean of the sample and the mean of the population 

**Alternative hypothesis ($H_1$)** is a **significant** deviation between the mean of the sample and the mean of the population 

**The p-level of significance** is the probability of obtaining such or an even stronger deviation from the mean value if the $H_0$ is true. The smaller $p$, the more reasons to reject the null hypothesis ($H_0)$. Usually at $p \leq 0.05$ we accept $H_1$, i.e. we got a a statistically significant deviation

**Type 1 Error** - $H_1$ is accepted, although $H_0$ are true
**Type 2 Error** - $H_0$ is accepted, although $H_1$ are true


## 2. Comparison of averages:
### 2.1 T-distribution

If the number of observations is small and unknown, then the **T-distribution** is used: unimodal, symmetric, but observations are more likely to fall outside the $\pm 2\sigma$ limit of the mean $M$ than the normal distribution.

The shape of the distribution is determined by the number of **degrees of freedom** ($df = n-1$). As $df$ increases, the distribution tends to be normal.

![[T-distribution_image.jpg]]


### 2.2 Comparison of two averages; Student's t-test

$$H_0: M_1 = M_2,\ H_1: M_1 \neq M2$$
$$
se = \sqrt{\frac{sd_1^2}{n_1} + \frac{sd_2^2}{n_2}},\ t = \frac{\bar X_1 - \bar X_2}{se}
$$
Knowing the number of degrees of freedom and the **t-value**, we can calculate the **p-level** of significance.