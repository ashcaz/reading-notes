# Linear Regression

**LINKS**

- [How to Run Linear Regression in Python](http://bigdata-madesimple.com/how-to-run-linear-regression-in-python-scikit-learn/)
- [Linear Regression in Python](https://realpython.com/linear-regression-in-python/)
- [Video: Introduction to Simple Linear Regressions](https://www.youtube.com/watch?v=KsVBBJRb9TE)
- [Train & Test Splits](https://towardsdatascience.com/train-test-split-and-cross-validation-in-python-80b61beca4b6)
- [What is Linear Regression](https://www.statisticssolutions.com/what-is-linear-regression/)

## How to Run Linear Regression in Python

Scikit-learn is a powerful Python module for machine learning. It contains function for regression, classification, clustering, model selection and dimensionality reduction. Today, I will explore the sklearn.linear_model module which contains “methods intended for regression in which the target value is expected to be a linear combination of the input variables”.

```Python
import numpy as np
import pandas as pd
import scipy.stats as stats
import matplotlib.pyplot as plt
import sklearn
```

Linear regression is a basic and commonly used type of predictive analysis. The overall idea of regression is to examine two things: (1) does a set of predictor variables do a good job in predicting an outcome (dependent) variable? (2) Which variables in particular are significant predictors of the outcome variable, and in what way do they–indicated by the magnitude and sign of the beta estimates–impact the outcome variable? These regression estimates are used to explain the relationship between one dependent variable and one or more independent variables.

[Back to Homepage](https://ashcaz.github.io/reading-notes)
