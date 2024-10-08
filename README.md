# TitanicML Project

This project applies various machine learning models to predict the survival of passengers on the Titanic.where the goal is to classify whether a passenger survived or not based on several features such as age, sex, ticket fare, and class.

## Overview
In this project, I have experiment with multiple machine learning algorithms including:
- Decision Tree Classifier
- K-Nearest Neighbors (KNN)


I have also perform hyperparameter tuning using Grid Search to find the best parameters for these models. The pipeline processes the data and then trains a model to predict survival, which is evaluated using various metrics.


## Dataset
The dataset contains data about Titanic passengers. The key features are:
- `Pclass`: Ticket class (1st, 2nd, or 3rd)
- `Sex`: Gender of the passenger
- `Age`: Age of the passenger
- `Fare`: Price of the ticket
- `Embarked`: Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- `SibSp`: Number of siblings or spouses aboard the Titanic
- `Parch`: Number of parents or children aboard the Titanic
- `Survived`: 0 = No, 1 = Yes (target variable)

### Files:
- `titanic_train.csv`: Training dataset used to train the models.
- `titanic_test.csv`: Test dataset used for model evaluation.

## Results
After tuning the models and evaluating them, here are the best scores achieved:

| Model              | Accuracy | Precision | Recall | F1 Score |
|--------------------|----------|-----------|--------|----------|
| Decision Tree       | 0.85     | 0.78      | 0.77   | 0.78     |


**Best Parameters**:  
```python
{
    'criterion': 'entropy',
    'max_depth': 50,
    'min_samples_leaf': 4,
    'min_samples_split': 10
}
