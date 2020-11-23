# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis: 
-  The business of predicting which loans will perform during the duration of the terms and which ones will be non-performers is a key area of interest to those in the banking industry. Afterall, a performing loan is a profitable venture, while a non-performing loan is not.  In order to try to create a predictive model, we created Machine Learning predictive models utilizing **over-sampling** (naive-random over-sampling & SMOTE), **under-sampling** (Cluster centroids), as well as the ensemble methods **Basic Random Forest Classifier** (which uses bagging) and finally **Easy Ensemble Adaboost Classifier** (which uses boosting).  Trying out multiple models and methods allowed us to compare their predictive results head to head, with their respective balanced accuracy scores, predictive and recall scores as our tools of comparison.



## Results:

There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models (15 pt)

![Alt_text](https://github.com/Nickguild1993/Credit_Risk_Analysis/blob/main/ML_tabled_scores.png)

Above is a table that shows all the scores for the 6 different models we fitted.  

- Both of the ensemble techniques (Adaboost & BasicRandomForest) performed at a higher level than any other type of model, be it under-sampling, over-sampling, or combination.  

- 

Adaboost scores - pre 1.00, rec .76, acc .72

BasicRandomForest - pre 1.00, rec .84, acc .71

SMOTEENN (combo)- pre 1.00, rec .57, acc .64

Cluster Centroids (under) - pre 1.00, rec .41, acc .547

SMOTE (over) - pre 1.00, rec .67, acc .655

Naive random over-sampling - pre 1.00, rec .66, acc .68






## Summary:

There is a summary of the results (2 pt)

There is a recommendation on which model to use, or there is no recommendation with a justification (3 pt)
