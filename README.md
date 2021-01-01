# Credit-Card-Application-Approval-Prediction

**Project**

* The goal of this project is to build a model to predict whether a customer's credit is good or bad based on their application data. 

* The label good/bad in the data were not pre-defined. Instead, only credit history of past customers were given.

* The link to the dataset can be found at: https://www.kaggle.com/rikdifos/credit-card-approval-prediction

**Kaggle notebooks**

* EDA: https://www.kaggle.com/hungndo/credit-modeling-eda

* Final models: https://www.kaggle.com/hungndo/credit-modeling-models

**Results**

* In this project, we performed different feature engineering, transformations, over/downsampling methods to train a model to classify good/bad credits with the provided unbalanced dataset.

* For model selection, we use f05 score as the main criteria to deal with this unbalanced data.
    
* From the 4 models we tried to train, Logistic Regression, KNN, and RandomForest produce similar results for cross validation. Random Forest has lower f05 score than others. For potential future needs for inferencing, we select the fitted Logistic Regression as the final model. Then, we run the Logistic Regression with the test set and it produces a similar result to its CV f05 score, which is about 0.8.
    
* WOE transformation didn't show much effect on the Logistic Regression, probably because we only performed transformation on categorical variable with cardinality lower than 20, left out the ones with high cardinality and continuous variable.

**Contributors**
* Hung Do
* Duy Bao Le
* Duy Nhat Le
* Jared Kaplan
* Joseph Tan
* Asim Thapa

**Acknowledgements**
* https://www.kaggle.com/rikdifos/eda-vintage-analysis
* https://www.listendata.com/2015/03/weight-of-evidence-woe-and-information.html
