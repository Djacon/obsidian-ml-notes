**Classification** is a [[machine learning]] algorithm in which the target label "$y$" is predicted using various features $X$. The input data can be anything, including continuous numbers, text, pictures, etc., while the output should be an **integer (discrete value)**

#### List of the main classification algorithms in ML:

1. [[Logistic Regression]]
2. Linear Discriminant Analysis (LDA)
3. [[GaussianNB]]
4. [[DecisionTreeClassifier]]
5. [[RandomForestClassifier]]
6. [[KNeighborsClassifier]]
7. [[Support Vector Classification]] (SVC)


#### List of basic [[Metric]] for Classification:

1. [[Accuracy]]
	* $\mbox{Accuracy} = \frac{1}{n}\sum_{i=1}^n[\hat y_i = y_i]$
2. [[Precision]]
	* $\mbox{Precision} = \frac{TP}{TP+FP} = \frac{\sum\ [\hat y_i = y_i = n]}{\sum\ [\hat y_i = n]}$
3. [[Recall]]
	* $\mbox{Recall} = \frac{TP}{TP+FN} = \frac{\sum\ [\hat y_i = y_i = n]}{\sum\ [y_i = n]}$
4. [[F-score]]
	* $F_1 = \frac{2}{\mbox{precision}^{-1} + \mbox{recall}^{-1}}$
1. [[Log-Loss]] (Binary Cross Entropy, BCE)
	* $BCE = -\frac{1}{n}\sum_{i=1}^n(y_i \log{\hat y_i} + (1 - y_i)\log{(1 - \hat y_i}))$