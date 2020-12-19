# MachineLearning_17

Credit risk was analyzed using a dataset.  The dataset was split into training and testing.  The set was unbalanced with relatively few bad loans.  Therefore, various sampling strategies were employed to try and improve model results. 

## Methodology

The following steps were employed: 
- clean the data - drop columns that are not independent, convert some columns to numerical values etc, scaled the data 
- Sample the data using four different methodologies
- Use logistic regression to make predictions and evaluated model performance
- Calculate the accuracy of the model 
- Generate a confusion matrix
- print out the inbalanced classification report

## Results 

The sampling strategy is the ratio of the minority to the majority population.  A ratio of 1 means a balance between the two.  A ratio of 1 seemed to work best for the oversampling.  A ratio nearly to 0.5 yielded better results for the undersampling and over/under sampling.

Balanced accuracy scores: 
- Naive random oversampling: 70
- Smote oversampling: 70
- Cluster Centriods undersampling:  69
- Over and undersampling, sampling strategy:  69
- Balanced random forest classifier: 82
- Adaptive boost classifier: 99

Adaptive boosting appears to be the best, but this was mainly becauase of the very high classification rate for low-risk customers.  The number of high risk customers was poorly identified.

Probably the more important thing to consider if the number of false positives - ie the customers who are actually credit risks, but who are classified as low risk.  This will directly lead to bad financial outcomes for the lender.  The number of "lost" low-risk customers is less of an issue.   The number of high risks incorrectly identified as low risk by various sampling methods includes: 

Bad customers who received loans (ie high risk who were predicted as low risk):  
- Naive random oversampling: 35
- Smote oversampling: 36
- Cluster Centriods undersampling:  35
- Over and undersampling, sampling strategy:  35
- Balanced random forest classifier: 39
- Adaptive boost classifier: 78





### Naive oversampling results
![1](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/Naive_oversample.png)

### Smote oversampling results
![2](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/smote_over.png)


### Undersampling Cluster Centroids
![3](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/under.png)

### Over and undersampling
![4](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/over_under.png)



# #Methodologies (Deliverable 3)

Two different ensemble classifiers were used to predict credit risk and evaluate each model. 






### Balanced random forest classifier

![5](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/UBRF1.png)

### Adaptive Boosting

![6](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/adaptiveboost.png)
![7](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/adaptiveboost2.png)


## Results

The various sampling strategies all resulted in similar balanced accuracy scores of 69 to 99%.  All the strategies were sensitive to the ratio of minority to majority samples that were set.  Balanced random forest was a good balance of correctly identifying the low risk customers and finding a good portion of the low risk.


