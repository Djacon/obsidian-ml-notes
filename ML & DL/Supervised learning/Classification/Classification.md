**Classification** is a [[machine learning]] algorithm in which the target label "$y$" is predicted using various features $X$. The input data can be anything, including continuous numbers, text, pictures, etc., while the output should be an **integer (discrete value)**

#### List of the main classification algorithms in ML:

1. [[Logistic Regression]]
2. Linear Discriminant Analysis (LDA)
3. Naive Bayes
4. Decision Tree Classifier
5. Random Forest Classifier
6. KNN
7. Support Vector Classification (SVC)


#### List of basic [[Metric]] for Classification:

1. [[Accuracy]]
	* $Accuracy = \frac{1}{n}\sum_{i=1}^n[\hat y_i = y_i]$
2. Precision
	* -
3. Recall
	* -
4. F1-score
	* - 
5. [[Log-Loss]] (Binary Cross Entropy, BCE)
	* $BCE = -\frac{1}{n}\sum_{i=1}^n(y_i \log{\hat y_i} + (1 - y_i)\log{(1 - \hat y_i}))$