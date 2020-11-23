# Credit_Risk_Analysis

## Overview of the loan prediction risk analysis: 
-  The business of predicting which loans will perform during the duration of the terms and which ones will be non-performers is a key area of interest to those in the banking industry. Afterall, a performing loan is a profitable venture, while a non-performing loan is not.  In order to try to create a predictive model, we created Machine Learning predictive models utilizing **over-sampling** (naive-random over-sampling & SMOTE), **under-sampling** (Cluster centroids), as well as the ensemble methods **Balanced Random Forest Classifier** (which uses bagging) and finally **Easy Ensemble Adaboost Classifier** (which uses boosting).  Trying out multiple models and methods allowed us to compare their predictive results head to head, with their respective balanced accuracy scores, predictive and recall scores as our tools of comparison.



## Results:


![Alt_text](https://github.com/Nickguild1993/Credit_Risk_Analysis/blob/main/ML_tabled_scores.png)

Above is a table that shows all the respective scores for the 6 different models we fitted.  

- Both of the ensemble techniques (Adaboost & BalancedRandomForest) performed at a higher level than any other type of model, be it under-sampling, over-sampling, or combination.  

- Both of the over-sampling models performed second best as a group overall, beating the scores of both the SMOTEENN (combination) and Cluster-Centroids (under-sampling)

- The combination method- SMOTEENN, performed next best, beating out Cluster Centroids to avoid last place.

- The model that performed the worst across the board was the Cluster Centroids, with both the lowest **recall** score, at .41, andlowest **accuracy** score, at .547

![alt_text](https://github.com/Nickguild1993/Credit_Risk_Analysis/blob/main/forest__top5_importance.png) 

- The above chart shows the 5 most important variables for predicting if a loan will default or not.  With the caveat that I am not a banker, those features having relatively high predictive value makes sense.  For example, the strongest indicator- the amount paid towards the oringinal principle at signing, is a feature that makes sense to have a relationship with the target.  Let's say you pay $20,000 over the minimum priniciple amount at the time of signing, not only are you reducing the amount of money left on the loan that can accumulate interest, you're also demonstrating that you have more than enough liquidity to afford the loan you're agreeing to.


## Summary:

![alt_text](https://github.com/Nickguild1993/Credit_Risk_Analysis/blob/main/Forest_ensemble_scores.png)

- Overall none of the models we configured are overly impressive in their metrics.  However, the **BalancedRandomForest** (which is shown above) had the highest scores overall, and given the nature of how Ensemble Learning works, having a system that doens't rely on a single model should return you less variance and errors, along with a higher overall accuracy level.   


