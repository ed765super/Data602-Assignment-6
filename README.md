# DATA602 Model Evaluation
## Data = pima_indian_data.csv

## Project Description:
The following will be done to the Pima Indian dataset

* Inspect the data and create a pipeline to perform any feature processing
* Prior to building the feature pipeline, be sure to split the data into training/test sets
* Create a logistic regression model pipeline that uses the above pipeline
* Pick a metric you are going to use to select the model and justify your choice.
* Use the above combined pipeline to run a Logistic Regression model with grid search cross-validation using 10 folds. Search 5 different regularization strengths and 2 solvers. 
* What is the best model?
* Answer the question: How does it perform on the test set?

All of this will be done while im predicting the class column

## EDA Findings
This is a solid 768 row × 9 column dataset with no missing values. Only a few of those columns have uniform distributions wwhile the rest are skewed in some way shape or form. All of the data is numerical with a small variatiion of scale. There is no notable multicoliniarity in this dataset.


## Regression Results
Cross Validation alone with no grid search produced a higher recall than either solvers that utilized grid search. LibLinear and Newton-cg chose the same regression strength and number of components. This is understandable as the dataset is rather small and the smaller the dataset the better the grid search cross validation is.

## Future plans
I would research all the other metrics available and  each one's subclasses. Each of the submetrics seemed to have small variations in how they're calculated and what they take into account. Perhaps by using a more specific form of recall I could find more useful information to evaluate the model.
