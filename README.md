# Credit_Risk_Analysis
You can find the Analysis file here: [credit_risk_resampling.ipynb](https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/credit_risk_resampling.ipynb) | [credit_risk_ensemble.ipynb](https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/credit_risk_ensemble.ipynb)
## Analysis Overview

## Results (Balanced Accuracy Scores, Confusion Matrixes and Imbalanced Classification Reports)

### RandomOverSampler model

<p align="center">
  <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/RandomOverSampler_BAS.PNG"> <br> <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/RandomOverSampler_CM.PNG"><img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/RandomOverSampler_Classification_report.PNG">
</p>
A balanced accuracy score of 64 percent is achieved.
The high risk precision is just approximately 1% with a sensitivity of 62 percent, resulting in an F1 of about 2%.
Because of the large number of low-risk people, it has a precision of almost 100 percent and a sensitivity of 68 percent.

### SMOTE model
<p align="center">
  <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20_BAS.PNG"> <br> <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/SMOTE%20_CM.PNG"><img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/SMOTE_Classification_report.PNG">
</p>
The outcomes are very similar to those of the prior model.
The balanced accuracy score is 63%.
The high risk precision is just approximately 1% with a sensitivity of 60 percent, resulting in an F1 of about 2%.
Because of the large number of low-risk individuals, it has an accuracy of almost 100% and a sensitivity of 68%.

### ClusterCentroids model
<p align="center">
  <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids_BAS.PNG"> <br> <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids_CM.PNG"><img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/ClusterCentroids_Classification_report.PNG">
</p>
Here the balanced accuracy score is down to about 51%. The high risk precision is still 1% with a sensitivity of 60 percent, resulting in an F1 of 1%.
The low risk sensitivity is just 43% due to the significant amount of false positives.

### SMOTEENN model
<p align="center">
  <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN%20_BAS.PNG"> <br> <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN%20_CM.PNG"><img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/SMOTEENN_Classification_report.PNG">
</p>
The balanced accuracy score is around 62%.
The high risk precision is still 1% with a sensitivity of 70 percent, resulting in an F1 of only 2%.
The low risk sensitivity is 55 percent due to the significant amount of false positives.

### BalancedRandomForestClassifier model
<p align="center">
  <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier_BAS.PNG"> <br> <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier_CM.PNG"><img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/BalancedRandomForestClassifier_Classification_report.PNG">
</p>
The balanced accuracy score increased to around 79%.
The high risk precision is still poor, at just 4% with only 67 percent sensitivity, resulting in an F1 of only 7%.
The low risk sensitivity is now 91 percent with 100 percent presicion, thanks to a decreasing number of false positives.

### EasyEnsembleClassifier model
<p align="center">
  <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier%20_BAS.PNG"> <br> <img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier%20_CM.PNG"><img src="https://github.com/NedaAJ/Credit_Risk_Analysis/blob/main/Resources/EasyEnsembleClassifier%20_Classification_report.PNG">
</p>
The balanced accuracy score has now risen to over 92 percent.
The high risk precision is still poor, at just 7% with 91 percent sensitivity, resulting in an F1 of of 14%.
The low risk sensitivity is now 94 percent with 100 percent precision, thanks to a decreasing number of false positives.

## Summary
All of the credit risk analysis models have low accuracy in assessing if a credit risk is high.
The Ensemble models resulted in significant improvements, particularly in the sensitivity of high-risk loans.
With a recall of 92 percent, the EasyEnsembleClassifier model can detect virtually all high-risk credit. On the other hand, because of the poor accuracy, many low-risk credits are still misclassified as high-risk, putting the bank's credit strategy at risk and causing it to miss out on income prospects.
As a result, I would advise the bank against using any of these algorithms to anticipate credit risk.

## Contact:
- Email : [neda.ahmadi.jesh@gmail.com](mailto:neda.ahmadi.jesh@gmail.com?subject=[GitHub]%20Source%20Han%20Sans)
- Linkedin: www.linkedin.com/in/neda-ahmadi-j
