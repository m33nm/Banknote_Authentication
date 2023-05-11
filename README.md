# Banknote_Authentication
Banknote authentication model using classification machine learning techniques involves the application of K-Nearest Neighbor and Artificial Neural Network 
classification algorithms to build machine learning models that predict whether a given banknote is authentic or forged, using 1,372 extracted measures 
(Variance, Skewness, Kurtosis, and Entropy) from both types of banknote images. Exploratory data analysis and preparation techniques were applied to the dataset.

All the variables are on different dimensions, and different scales of the data features can affect the modeling of a dataset. Thus, I normalized the features
to a standard range to achieve an acceptable result. SMOTE (Synthetic Minority Oversampling Technique) resampling method was applied to handle the data class
imbalance. However, the models were developed using both balanced and unbalanced dataset to compare the performance of each. 

# Results Analysis and Discussion
In evaluating the performance of the banknote authentication models, the model must identify as many forged notes (positive class) as possible for it to be 
reliable. False Negative is of a more significant concern than False Positive in this scenario; thus, a model with a high recall, f1-score, and accuracy is best
suited for the task. The tables below summarize the results of each classification algorithm applied to the dataset.

![image](https://github.com/m33nm/Banknote_Authentication/assets/54365936/ad742b44-b3c2-474f-aec7-e4f74aab4fb4)
Table 1: Performance metrics for KNN and ANN Classification Algorithms
![image](https://github.com/m33nm/Banknote_Authentication/assets/54365936/0d59c83a-cd47-45e3-8b6a-7199237e12fb)
Table 2: Confusion matrix for KNN and ANN Classification Algorithms

# Conclusion
KNN and ANN (version 3, with balanced data and increased epoch) models have exceedingly good results. But in comparison, KNN performs better than ANN based on 
the results obtained. KNN accurately identified all the positive classes with a 100% recall. Although the KNN algorithm performs better with large training data,
I recommend extensive analysis of more feature instances for future deployment.
