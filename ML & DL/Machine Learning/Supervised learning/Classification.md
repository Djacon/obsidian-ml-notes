**Classification** is a [[machine learning]] algorithm in which the target label "$y$" is predicted using various features $X$. The input [[data]] can be anything, including continuous numbers, text, pictures, etc., while the output should be an **integer (discrete value)**

#### List of the main classification algorithms in ML:

* [[Logistic Regression]]
* [[GaussianNB]]
* [[DecisionTreeClassifier]]
* [[RandomForestClassifier]]
* [[KNeighborsClassifier]]
* [[Neural Network]]
* [[Support Vector Classification]] (SVC)

#### List of basic [[Metric]] for Classification:

* [[Accuracy]]
	* $\mbox{Accuracy} = \frac{1}{n}\sum_{i=1}^n[\hat y_i = y_i]$
* [[Precision]]
	* $\mbox{Precision} = \frac{TP}{TP+FP} = \frac{\sum\ [\hat y_i = y_i = n]}{\sum\ [\hat y_i = n]}$
* [[Recall]]
	* $\mbox{Recall} = \frac{TP}{TP+FN} = \frac{\sum\ [\hat y_i = y_i = n]}{\sum\ [y_i = n]}$
* [[F-score]]
	* $F_1 = \frac{2}{\mbox{precision}^{-1} + \mbox{recall}^{-1}}$
* [[Log-Loss]] (Binary Cross Entropy, BCE)
	* $BCE = -\frac{1}{n}\sum_{i=1}^n(y_i \log{\hat y_i} + (1 - y_i)\log{(1 - \hat y_i}))$