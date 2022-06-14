# Decision-Trees

Decision Trees are a non-parametric supervised learning method used for [classification](https://www.geeksforgeeks.org/ml-classification-vs-regression/) and [regression](https://www.geeksforgeeks.org/ml-classification-vs-regression/). The goal is to create a model that predicts the value of a target variable by learning simple decision rules inferred from the data features.


Dcision trees learn from data to approximate a sine curve with a set of if-then-else decision rules. The deeper the tree, the more complex the decision rules and the fitter the model.


## Clssification 

DecisionTreeClassifier is a class capable of performing multi-class classification on a dataset.

DecisionTreeClassifier takes as input two arrays: an array X, sparse or dense, of size [n_samples, n_features] holding the training samples, and an array Y of integer values, size [n_samples], holding the class labels for the training samples.

![download (2)](https://user-images.githubusercontent.com/55234691/91148399-33d25180-e6d7-11ea-8bde-ca6da300465b.png)

I can also export the tree in Graphviz format using the export_graphviz exporter. 

installed with **conda install python-graphviz**

![iris](https://user-images.githubusercontent.com/55234691/91150980-b27cbe00-e6da-11ea-80a5-45b18e9059ab.png)


## Regression 

The decision trees is used to fit a sine curve with addition noisy observation. As a result, it learns local linear regressions approximating the sine curve.

I can see that if the maximum depth of the tree (controlled by the max_depth parameter) is set too high, the decision trees learn too fine details of the training data and learn from the noise, i.e. they overfit.


![download](https://user-images.githubusercontent.com/55234691/91151405-3e8ee580-e6db-11ea-877f-57d214f35331.png)

## Multi-output Decision Tree Regression

The decision trees is used to predict simultaneously the noisy x and y observations of a circle given a single underlying feature. As a result, it learns local linear regressions approximating the circle.

The maximum depth of the tree (controlled by the max_depth parameter) is set too high, the decision trees learn too fine details of the training data and learn from the noise, i.e. they overfit.

![download (1)](https://user-images.githubusercontent.com/55234691/91152109-2bc8e080-e6dc-11ea-8145-85bf491a7d87.png)
