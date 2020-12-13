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
