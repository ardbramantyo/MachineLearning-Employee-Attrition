### Comparative Machine Learning Method to Predict Employee Attrition
Data Source: [Kaggle](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
### Overview
The project is aimed to develop Machine Learning models and make comparative prediction from employees data (1470 rows data) that could better predict Employees attrition.

**Tools:** Pandas, Numpy, Seaborn, Matplotlib, Scikit-Learn, Tensorflow, Keras

#### Data Cleaning
To avoid AI misunderstanding, 2 variables are made based on their data type.
1. Categorical: Anything from fields exclude Attrition  object data type
2. Numerical:  Anything from fields with numerical data type.

Converting Categorical variable data type using scikit-learn into number:
``` ruby
from sklearn.preprocessing import OneHotEncoder
onehotencoder = OneHotEncoder()
X_cat = onehotencoder.fit_transform(X_cat).toarray()
```
### Model Accuracy Test Method:
1. Logistic Regression
2. Random Forest
3. Deep Learning Model 

### Accuracy measurement:
 - Training: 1102 (75%)
 - Test: 368 (25%)

### 1. Logistics Regression Evaluation
Accuracy 88.56%

### 2. Random Forest Evaluation

### 3. Deep Learning Model Evaluation

![image](https://user-images.githubusercontent.com/37673834/169192599-d06e652a-7a06-4309-b9e5-d2f6e7eab3ff.png)


### Comparison

![image](https://user-images.githubusercontent.com/37673834/169203314-84f5b0e0-2406-4e74-af64-d9022e0f4da9.png)
Confusion Matrix: Logistic Regression(left), Random Forest(mid), Deep Learning(right)

|   Method           |Accuracy (%)|
|--------------------|------------|
| Logistic Regression|         89 |
| Random Forest      |         85 |
| Deep Learning      |         83 |

### Reference:
1. https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset
2. https://matplotlib.org/3.5.0/plot_types/index.html
3. https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html
4. https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.OneHotEncoder.html
5. https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html
6. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.accuracy_score.html
7. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html
8. https://scikit-learn.org/stable/modules/generated/sklearn.metrics.classification_report.html
9. https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html
10. https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html
11. https://seaborn.pydata.org/generated/seaborn.heatmap.html
12. https://seaborn.pydata.org/generated/seaborn.countplot.html
13. https://seaborn.pydata.org/generated/seaborn.kdeplot.html
14. https://www.tensorflow.org/api_docs/python/tf/keras/Sequential
15. https://www.tensorflow.org/guide/keras/train_and_evaluate
16. https://www.tensorflow.org/api_docs/python/tf/keras/Model
17. https://www.tensorflow.org/api_docs/python/tf/keras/layers/Dense
18. https://towardsdatascience.com/a-practical-guide-to-implementing-a-random-forest-classifier-in-python-979988d8a263
