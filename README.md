# MachineLearning_17

Credit risk was analyzed using a dataset.  The dataset was split into training and testing.  The set was unbalanced with relatively few bad loans.  Therefore, various sampling strategies were employed to try and improve model results. 

## Sampling methodologies (Deliverable 1 & 2)

The following steps were employed: 
- sample the data using the various methodologies
- Use logistic regression to make predictions and evaluated model performance
- Calculate the accuracy of the model 
- Generate a confusion matrix
- print out the inbalanced classification report


The sampling strategy is the ratio of the minority to the majority population.  A ratio of 1 means a balance between the two.  A ratio of 1 seemed to work best for the oversampling.  A ratio nearly to 0.5 yielded better results for the undersampling and over/under sampling.
- Naive random oversampling, sampling_strategy = 1, balanced accuracy score = 0.65
- Smote oversampling, sampling_strategy = 1, balanced accuracy score = 0.66
- Cluster Centriods undersampling, sampling strategy = 0.5, balanced accuracy score = 0.65
- Over and undersampling, sampling strategy = 0.5, balanced accuracy score = 0.65

### Naive oversampling results
![1](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/Naive_oversample.png)

### Smote oversampling results
![2](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/smote_over.png)


### Undersampling Cluster Centroids
![3](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/under.png)

### Over and undersampling
![4](https://github.com/JaniceBgithub/MachineLearning_17/blob/main/Resources/over_under.png)


## Sampling Methoodology Results

The various sampling strategies all resulted in similar balanced accuracy scores of 0.65 to 0.66.  All the strategies were sensitive to the ratio of minority to majority samples that were set.   The F1 figure was around 0.81 for all cases, except for naive undersampling which had an F1 score of 0.75.

