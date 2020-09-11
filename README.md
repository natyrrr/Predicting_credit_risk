#  Risky Business- Predicting Credit Risk
Predicting credit risk using several machine learning models. Using Lending club data.

## *BACKGROUND*
Auto loans, mortgages, student loans, debt consolidation ... these are just a few examples of credit and loans that people are seeking online. Peer-to-peer lending services such as LendingClub or Prosper allow investors to loan other people money without the use of a bank. However, investors always want to mitigate risk, so you have been asked by a client to help them use machine learning techniques to predict credit risk.

I will build and evaluate several machine-learning models to predict credit risk using free data from LendingClub. Credit risk is an inherently imbalanced classification problem (the number of good loans is much larger than the number of at-risk loans), so I will need to employ different techniques for training and evaluating models with imbalanced classes. I will use the imbalanced-learn and Scikit-learn libraries to build and evaluate models using the two following techniques:
## Resampling 

### QUESTIONS TO BE ANSWERED

Which model had the best balanced accuracy score?
Which model had the best recall score?
Which model had the best geometric mean score?

### PROCESS
1.Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2.Oversample the data using the Naive Random Oversampler and SMOTE algorithms.
3.Undersample the data using the Cluster Centroids algorithm.
4.Over- and under-sample using a combination SMOTEENN algorithm.

*For each of the above, I will:*

1.Train a logistic regression classifier from sklearn.linear_model using the resampled data.
2.Calculate the balanced accuracy score from sklearn.metrics.
3.Calculate the confusion matrix from sklearn.metrics.
4.Print the imbalanced classification report from imblearn.metrics.

## Ensemble Learning

### QUESTIONS TO BE ANSWERED
Which model had the best balanced accuracy score?
Which model had the best recall score?
Which model had the best geometric mean score?
What are the top three features?
 
### PROCESS

1.Load the Lending Club data, split the data into training and testing sets, and scale the features data.
2.Train the model using the quarterly data from LendingClub provided in the Resource folder.
3.Calculate the balanced accuracy score from sklearn.metrics.
4.Print the confusion matrix from sklearn.metrics.
5.Generate a classification report using the imbalanced_classification_report from imbalanced learn.
6.For the balanced random forest classifier only, print the feature importance sorted in descending order (most important feature to least important) along with the feature score.


## CONCLUSION AND FINAL ANSWERS.

#### RESAMPLING

Which model had the best balanced accuracy score? 
#### *Naive random oversampling had the best score with .67, while SMOTE had a balanced accuracy score with .64.Combination had a balance score of .64 and undersampling had a score of .54.*

Which model had the best recall score? 

#### *Both Naive random oversampling and SMOTE had the same mean recall score with high risk being .63 and low risk being .69.*

Which model had the best geometric mean score?

**Naive and SMOTE both had the best score with .66 mean score.**

### ENSEMBLE LEARNING:

Which model had the best balanced accuracy score?

#### *The Easy Ensemble had the best balance accuracy score of .93, while the random forest had an accuracy score of .78.*

Which model had the best recall score?

#### *The Easy ensemble had the best recall with a mean of .94 while random forest had a mean of .90. In easy ensemble both low risk and high risk had high recall scores while in random forest the high risk had a much lower score than low risk with .67 to .90.*

Which model had the best geometric mean score?

#### *The easy ensemble classifier had the best geometric score with .93.*

What are the top three features?

#### *Precision, recall, and specificity*
