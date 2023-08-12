# ML-CourseProject
 ### Estimation of obesity levels using Machine Learning models (Random Forest) : 
 As one of the supervised machine learning algorithms that is frequently used in 
classification and regression, we have selected the Random Forest classification model 
for our project. It is integrated into multiple decision trees as opposed to just one, and 
the decision tree with the most votes is chosen based on each tree's projected outcome. 
One of a random forest's key characteristics is its ability to handle data sets with both 
continuous and categorical variables for classification and regression. Because of its 
implementation flexibility and our prior experience, we chose Random Forest.


### Goal State :
Our aim is to classify the Level of Obesity of individuals based on estimation features 
given. in addition, there is an "insufficient weight", which indicates that the model 
does not have information to determine the obesity level. 
Our main goal is to build a ML model, train it and make it estimate the Level of Obesity of 
individuals, by Random Forest model.

###  Discussion :
As we explained above, with and without feature selection we noticed in both that the 
training model reaches 100%, which means that there is overfitting.
Avg test accuracy without feature selection without hyperparameter tuning: 95.39431%
Avg test accuracy with feature selection without hyperparameter tuning: 96.2303%
With unseen data it was better with feature selection, as it reduced the gap between 
testing and training model, by using feature_importance
Feature importance is calculated as the decrease in node impurity weighted by the 
probability of reaching that node. The node probability can be calculated by the number 
of samples that reach the node, divided by the total number of samples. The higher the 
value the more important the feature. However, this happens technically within the code.

And to solve the problem of overfitting, we decided to do the optimization through the 
hyperparameter tuning using GridsearchCV, and one of the solutions used is determine 
the depth values.
Avg training accuracy with feature selection with hyperparameter tuning: 95.42994%
Avg test accuracy with feature selection with hyperparameter tuning: 92.01894%
Avg training accuracy without feature selection with hyperparameter tuning :96.1679%
Avg test accuracy without feature selection with hyperparameter tuning :92.11358% 
This enhances performance, even though the differences are very small.
So, with feature selection and the hyperparameter tuning, the performance will be better 
because the hyperparameter tuning without feature selection may take a long time 
We have benefited from applying feature selection, which will reduce the time 
complexity of the model and less possibility of overfighting.

### Conclusion : 
In conclusion, we presented our work in this project an Obesity Level Estimator application 
using Random Forest model. We faced several challenges since it is our first time to deal 
with Random Forest model, also the time taken to find a suitable dataset to implement our 
project, search/understanding the python libraries and function. After searching and 
learning we tries to train the model perfectly. Overall results shows that the model shows 
good prediction results with average of 95.42994% train accuracy and 92.01894% test 
accuracy.

## For details, visit our project on Google Colab .
