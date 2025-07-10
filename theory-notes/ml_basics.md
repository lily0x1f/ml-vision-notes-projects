# ML Models Basics
### Linear Regression
### Loss Functions
It is the method evaluating how well an algorithm models the dataset. (Compares predictions and actual data)

Different types of loss functions

Mean Squared error

<img width="311" height="112" alt="image" src="https://github.com/user-attachments/assets/733c42d5-ddf9-4211-a463-617d0a2c401a" />

What is outlier? -> check this

### Gradient Descent

An optimization technique to minimize the loss iterativly change wight and bias. 

### loss curve
Helps determining when model is converging or overfitting. 

Loss functions for linear models produce a convex surface->check this

HYPERPARAMETERS

Values we can control are hyperparameters.(external configuration) -> model architecture, learning rate, model complexity, epoch, batch size
Tuning them is important (check when learning rate is too high model bounces) -> techniques for tuning Bayesian optimization, Grid search, Random search...
````
check the directory named fundamental libraries
````


### Logistic Regression

Logistic regression is a data analysis technique that uses mathematics to find the relationships between two data factors. It then uses this relationship to predict the value of one of those factors based on the other. The prediction usually has a finite number of outcomes, like yes or no.
<img width="276" height="84" alt="image" src="https://github.com/user-attachments/assets/cc92186b-36ac-422c-a87c-d9aea103c609" />

This is how logistic regression estimates the value of the dependent variabvle and.
Logistic regression momdels use Log Loss as the loss fucntion instead of squared loss. Regularization should be applied to prevent overfitting
<img width="564" height="71" alt="image" src="https://github.com/user-attachments/assets/5b39ebab-115d-4a2f-b9f4-6873a321a8d9" />

to learn regularization wait 


### Classification

Thresholds and the confusion matrix

You choose a classification threshold: below is not, above is yes

A confusion matrix is this:
<img width="687" height="504" alt="image" src="https://github.com/user-attachments/assets/33c45944-dc08-4982-8ceb-79d97ea880ac" />

Some metrics calculated using true and false positives and negatives:

### Accuracy
Accuracy is the proportion of all true classifications.
<img width="653" height="87" alt="image" src="https://github.com/user-attachments/assets/d09c8e00-3f65-4811-ac04-ae43e62785e1" />

This is often the default evaluation metric used for generic or unspecified models carrying out tasks. 
However when dataset  is imbalanced or one mistake is costly its better to optimize other metrics.

### Recall (true positive rate)
Recall is the proportion of all true positives to positives.

<img width="728" height="88" alt="image" src="https://github.com/user-attachments/assets/eac486f7-b486-41b1-b0a2-48acecea03b1" />

In an imbalanced dataset where the number of actual positives is very low, recall is more meaningful because it measures how good the predction on correctly identifying positive cases. 


### False positive rate
It is the proporstion of all actual negatives that were classified incorrectly as positives. (probability of false alarm)

<img width="728" height="88" alt="image" src="https://github.com/user-attachments/assets/904bbed3-7bad-447e-90ec-aaa2d7b67572" />

### Precision

Proportion of true positive to all positives

<img width="728" height="88" alt="image" src="https://github.com/user-attachments/assets/6a6c39c4-7e2b-4a63-8e44-6e94d1777654" />

Precision improves as false positives decrease, while recall improves when false negatives decrease. -> conflictingg

<img width="762" height="462" alt="image" src="https://github.com/user-attachments/assets/77330652-60f4-48e9-8a44-44bab7d46b3a" />
