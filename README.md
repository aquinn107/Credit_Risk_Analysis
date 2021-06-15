# Credit_Risk_Analysis

## Overview of the analysis: 
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we need to employ different techniques to train and evaluate models with unbalanced classes. We were asked to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling to evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

---

## Results: 
- Algorithm: RandomOverSampler
  - Accuracy Score: 0.63
  - Precision Score: 0.99
  - Recall Score: 0.64

![RandomOverSampler_classification_report](https://raw.githubusercontent.com/aquinn107/Credit_Risk_Analysis/main/RandomOverSampler_classification_report.png)
- Algorithm: SMOTE
  - Accuracy Score: 0.63
  - Precision Score: 0.99
  - Recall Score: 0.64

![SMOTE_imbalanced_report](https://raw.githubusercontent.com/aquinn107/Credit_Risk_Analysis/main/SMOTE_imbalanced_report.png)
- Algorithm: ClusterCentroids
  - Accuracy Score: 0.52
  - Precision Score: 0.99
  - Recall Score: 0.40

![ClusterCentroids_classification_report](https://raw.githubusercontent.com/aquinn107/Credit_Risk_Analysis/main/ClusterCentroids_classification_report.png)
- Algorithm: SMOTEENN
  - Accuracy Score: 0.61
  - Precision Score: 0.99
  - Recall Score: 0.54

![SMOTEENN_classification_report](https://raw.githubusercontent.com/aquinn107/Credit_Risk_Analysis/main/SMOTEENN_classification_report.png)
- Algorithm: BalancedRandomForestClassifier
  - Accuracy Score: 0.78
  - Precision Score: 0.99
  - Recall Score: 0.87
  
![RandomForest_classification_report](https://raw.githubusercontent.com/aquinn107/Credit_Risk_Analysis/main/RandomForest_classification_report.png)
- Algorithm: EasyEnsembleClassifier
  - Accuracy Score: 0.93
  - Precision Score: 0.99
  - Recall Score: 0.94

![EasyEnsemble_classification_report](https://raw.githubusercontent.com/aquinn107/Credit_Risk_Analysis/main/EasyEnsemble_classification_report.png)

## Summary: 
In summary, because of how low both scores are the Undersampling model is not recommended for credit card risk analysis.
For credit card analysis I would say the Easy Ensemble model would be the best recommended to use. It was able to produce both a high accuracy and F-1 score of 0.97 surpassing all other models tested.
