# Credit_Risk_Analysis
Overview of the Analysis:
Defaulting loans can be a major issue for creditors. Consequently, finding ways, especially through technology, to address these issues is a gateway to mitigating risks from the get-go by identifying which applicants pose a higher risk. This analysis uses a machine learning toolkit including algorithims such as RandomOverSampler, SMOTE, ClusterCentroids, and SMOTEENN as well as different ensemble classifiers such as BalancedRandomForestClassifier and EasyEnsembleClassifier. These algorithms help to identify low versus high risk loan applicants. 

Please find below a brief description of each algorithm and ensemble used --
RandomOverSampler: Used to randomly oversample in a minority class by selecting samples with replacement
SMOTE: Synthetic Minority Over-sampling Technique
ClusterCentroids: "Method that under samples the majority class by replacing a cluster of majority samples by the cluster centroid of a KMeans algorithm" (Imbalanced-learn.org)
SMOTEENN: "Combine over- and under-sampling using SMOTE and Edited Nearest Neighbours"(Imbalanced-learn.org)
BalancedRandomForestClassifier: "A balanced random forest randomly under-samples each boostrap sample to balance it."(Imbalanced-learn.org)
EasyEnsembleClassifier:"The classifier is an ensemble of AdaBoost learners trained on different balanced boostrap samples. The balancing is achieved by random under-sampling."(Imbalanced-learn.org)


Results:
The balanced accuracy scores are as follows -- Oversampling (0.67), SMOTE (0.68), Undersampling (0.52),SMOTEENN (0.68), Balanceed Random Forest Classifier (0.79), Easy Ensemble AdaBoost Classifier (0.93).

Oversampling had a precision of 99% and recall of 66%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/Oversampling.PNG)

SMOTE (Oversampling) had a precision of 99% and recall of 69%
----------------------------------------------- 
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/SMOTE.PNG)

Cluster Centroids had a precision of 99% and recall of 43%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids.PNG)

SMOTEENN had a precision of 99% and recall of 58%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/SMOTEEN.PNG)

Balanceed Random Forest Classifier had a precision of 99% and recall of 90%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.PNG)

Ensemble AdaBoost Classifier had a precision of 100% and recall of 94%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)

Summary:
 The methods used employed undersampling, oversampling as well as a combination of both. The accuracy proved to be higher with the ensemble algorithms. Within the other algorithms the most accurate was SMOTE at 0.683 followed by SMOTEEN at 0.679 (rounded to 0.68). As for the Ensemble Classifier, it deemed to be the most precise of all the algorithms attempted. Indeed, this proves to also be the most reliable given the equilibrium there is between accuracy as well as precision. 
