# Traditional Machine Learning

## Supervised Learning
In supervised learning, training involves labelled data.

### Classification
Given a set of independent variables, the class to which the example belongs to should be determined. The output in classification is discrete in nature.
- **Logistic Regression** : It makes use of a special function known as *sigmoid* function. Based on a threshold (usually P = 0.5) the class is determined.  
https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html 
https://www.aionlinecourse.com/tutorial/machine-learning/logistic-regression

- **K Nearest Neighbours Classification** : In this type of classification, we choose *K* nearest neighbours for the test data point and assign it to the class which contains maximum number of its *K* nearest neighbours.  
https://scikit-learn.org/stable/modules/generated/sklearn.neighbors.KNeighborsClassifier.html 
https://www.aionlinecourse.com/tutorial/machine-learning/k-nearest-neighbor

- **Support Vector Machine** : The classes are separated by an optimal hyperplane (margin between the classes is maximum). In other words it works by finding an optimal decision boundary.  
https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html   
https://www.aionlinecourse.com/tutorial/machine-learning/support-vector-machine

- **Naive Bayes Classification** : It is a probablilistic approach and as the name suggests is on the basis of Bayes theorem.  
https://scikit-learn.org/stable/modules/naive_bayes.html 
https://www.aionlinecourse.com/tutorial/machine-learning/bayes-theorem

- **Decision Tree Classification** :   
https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html
https://www.aionlinecourse.com/tutorial/machine-learning/decision-tree-classification

- **Random Forest Classification** :  
https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html  
https://www.aionlinecourse.com/tutorial/machine-learning/random-forest-classification 
