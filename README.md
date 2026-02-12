### SHIFT ML 2026 CHALLENGE
EDA challenge from SHIFT project

link: https://www.codabench.org/competitions/12921/

Datasets are excluded form the github repo, so you 
may fetch it from the competition site. 

Rules and targets:

![img.png](img.png)

In accordance of competition targets there was done:
- data clearance from duplicated and features, which don't 
have any analytical value, because they contaion only single 
value or ratio of such values in comparison with its total data
- object data types were evaluated and processed to meaningfull data
- categorical features were transformed to the number representation
(label encoding, transformation to timestamp or numerical meaningful values)
- features were checked for empty values and proceeded accordingly situation:
either dropped from the data set or replaced by mode value
- features were checked for the outliers and then was selected and applied normalizer
- numerical features were checked for the empty values and processed accordingly
- finally, the full list of the features were obtained
- built main EDA pipeline data processing function, which returns processed
and ready to used for model fitting train, validation and test datasets
- trained and validated the few most common sklearn binary classifiers as well 
as the catboost classifier
- since, the main competition metric is the ROC-AUC score, was compared that
score across all trained models and selected the best one
- selected model was used for test target prediction