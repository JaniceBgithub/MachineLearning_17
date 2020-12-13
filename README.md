# MachineLearning_17

Credit risk was analyzed using a dataset.  The dataset was split into training and testing.  The set was unbalanced with relatively few bad loans.  Therefore, various sampling strategies were employed to try and improve model results. 

## Methodology

The following steps were employed: 
- Sample the data using four different methodologies
- Use logistic regression to make predictions and evaluated model performance
- Calculate the accuracy of the model 
- Generate a confusion matrix
- print out the inbalanced classification report

## Results 

The sampling strategy is the ratio of the minority to the majority population.  A ratio of 1 means a balance between the two.  A ratio of 1 seemed to work best for the oversampling.  A ratio nearly to 0.5 yielded better results for the undersampling and over/under sampling.

Balanced accuracy scores: 
- Naive random oversampling: 31
- Smote oversampling: 37
- Cluster Centriods undersampling:  37
- Over and undersampling, sampling strategy:  37
- Balanced random forest classifier: 30
- Adaptive boost classifier: 63

Probably the more important thing to consider if the number of false positives - ie the customers who are actually credit risks, but who received loans.  The number for each of those by the various sampling methods includes: 

Bad customers who received loans:  
- Naive random oversampling: 0.65
- Smote oversampling: 0.66
- Cluster Centriods undersampling:  0.65
- Over and undersampling, sampling strategy:  0.65
- Balanced random forest classifier: 0.87
- Adaptive boost classifier: 0.99





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

### Confusion Matrix

![6](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/adaptiveboost.png)


## Results

The various sampling strategies all resulted in similar balanced accuracy scores of 0.65 to 0.66.  All the strategies were sensitive to the ratio of minority to majority samples that were set.   The F1 figure was around 0.81 for all cases, except for naive undersampling which had an F1 score of 0.75.


