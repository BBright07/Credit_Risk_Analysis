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

Oversampling had a precision of 99% and recall of 66%, and accuracy of 67%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/Oversampling.PNG)

SMOTE (Oversampling) had a precision of 99% and recall of 69%, and accuracy of 68%
----------------------------------------------- 
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/SMOTE.PNG)

Cluster Centroids had a precision of 99% and recall of 43%, and accuracy of 52%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/ClusterCentroids.PNG)

SMOTEENN had a precision of 99% and recall of 58%, and accuracy of 68%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/SMOTEEN.PNG)

Balanceed Random Forest Classifier had a precision of 99% and recall of 90%, and accuracy of 79%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/BalancedRandomForestClassifier.PNG)

Ensemble AdaBoost Classifier had a precision of 100% and recall of 94%, and accuracy of 93%
-----------------------------------------------
![Oversampling](https://github.com/BBright07/Credit_Risk_Analysis/blob/main/Images/Easy%20Ensemble%20AdaBoost%20Classifier.PNG)

Summary:
The methods used employed undersampling, oversampling as well as a combination of both. The findings highlighted overall high precision with variations in recall and accurracy across the board. Precision is the proportion of true positives over *actual* results while recall is the proportion of true positives over *predicted* results. The model with the best predictions was the Ensemble and the model with the worst prediction or recall was the Cluster model that used a combination of oversampling and undersampling. The model with the best precision is again the Ensemble model with all the other models falling behind by 1%. The decisive factor to identify the best model was therefore the measure for accuracy. The highest accuracy was identified in the Ensemble model at 93% and the lowest accuracy was at 52% for the Cluster Centroids model. Overall, the Ensemble AdaBoost Classifier was the most reliable model to identify credit client risk for creditors interested in integrating machine learning in their framework.
