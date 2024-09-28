# classification-challenge

# Dataset
The dataset consists of email data labeled as either spam or not spam. Each email is represented by a set of features (such as word_freq_make,	word_freq_addresss, etc.) which help the model learn to differentiate between spam and legitimate messages.

# Data Columns:
Features like email content, frequency of certain words, presence of specific characters, etc.
Target: A binary label (1 = Spam, 0 = Not Spam).
The dataset is split into:

# Training Data: Used to train the models.
Testing Data: Used to evaluate model performance.
Feature Scaling
To ensure that models like Logistic Regression & Random Forest perform optimally, the feature data was scaled using StandardScaler. Scaling helps in speeding up convergence and improving accuracy.

 # Models Used
1. Logistic Regression
A simple and interpretable linear model used for binary classification. Logistic Regression assigns probabilities to each class (spam or not spam) and classifies based on a threshold (typically 0.5).

2. Random Forest Classifier
An ensemble learning method based on decision trees. It builds multiple decision trees and aggregates their predictions (via voting in the case of classification) to improve the model's performance. This model is better suited for handling complex patterns in the data.

# Results
Model			Training Accuracy	Testing Accuracy
Logistic Regression	92.98%			92.87%
Random Forest		99.97%			96.70%
Logistic Regression: This model showed consistent performance between the training and testing sets, indicating good generalization but slightly lower accuracy compared to Random Forest.
Random Forest: This model performed better overall in terms of accuracy, but the gap between training and testing performance suggests potential overfitting.
