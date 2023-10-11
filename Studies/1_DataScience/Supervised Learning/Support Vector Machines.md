The idea behind the SVM is to create a decision boundary between two classes, this decision boundary can be both linear or non-linear function, it depends usually on how the dataset is disposed. Important to say that the SVM natively is used only for binary classification, but it has some additions to handle multi-classification tasks (Usually by breaking the multi-classification problem in multiple binary classification problems).

![[Pasted image 20231002103219.png]]

The algorithm steps in a higher abstraction level are:
- First we need to find the Support Vectors, which are the two nearest instances from different classes. 
- Then, we draw the hyperline/hyperplane that better divides the two classes by maximizing the margin between the support vectors.