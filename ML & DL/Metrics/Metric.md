**Metric** is a function for evaluating the performance of a particular [[Machine Learning]] algorithm. Each individual task may require a different metric, so you need to understand in which task to apply one or another metric

#### Hierarchy of metrics:
1. **Business metric** a metric based on the fact that we need to measure data at a point in time without having historical data (e.g. to predict the future revenue of a service)
2. **Online metric** a metrics based on a system already in operation, with which we hope to assess what will happen to business metrics
3. **Offline metric** a metric based on already known data, with which we can find the deviation of the model prediction from the true values of the target