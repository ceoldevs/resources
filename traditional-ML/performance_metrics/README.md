# Traditional Machine Learning

## Performance Metrics
```
TP = True Positive
TN = True Negative
FP = False Positive
FN = False Negative
```
- **Accuracy** : Use it when your data is balanced. $$\frac{TP + TN}{TP + FP + TN + FN}$$
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.accuracy_score.html

- **Precision** : Use it when False Positives are dangerous (Eg: Spam Detection) $$\frac{TP}{TP + FP}$$
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.precision_score.html

- **Recall** : Use it when False Negatives are dangerous (Eg: Cancer Prediction) $$\frac{TP}{TP + FN}$$
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.recall_score.html

- **F $\beta$ Score** : $$\frac{(1 + \beta) * recall * precision}{\beta^2 * (recall + precision)}$$ 
If both FN and FP are equally important, use $\beta = 1$.  
Else If FP is more important than FN, use $0 < \beta < 1$  
Else, use $2 < \beta < 10$  
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.fbeta_score.html

- **Confusion Matrix** : $$\begin{bmatrix}TN & FP\\ FN & TP\end{bmatrix}$$
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.confusion_matrix.html

- **ROCAUC** : It is *Area Under Receiver Operating Characteristic Curve* shows the performance of classification models. In ROC graph, TPR (True Positive Rate) is plotted against FPR (False Positive Rate). A classification model is said to be good if the area under ROC curve is high.  
https://developers.google.com/machine-learning/crash-course/classification/roc-and-auc
https://scikit-learn.org/stable/modules/generated/sklearn.metrics.roc_auc_score.html
