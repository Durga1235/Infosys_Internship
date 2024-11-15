# Heart Stroke Prediction Project 

This project aims to compare multiple machine learning models to predict the risk of heart stroke in patients. In this milestone, we focused on building and evaluating four models: **Linear Regression**, **Lasso Regression**, **Ridge Regression**, and **Logistic Regression**. We compared these models based on **Accuracy** and **Root Mean Square Error (RMSE)** to understand their effectiveness in predicting stroke occurrences.

## Table of Contents

- [Project Overview](#project-overview)
- [Models Used](#models-used)
- [Mathematics Behind Models](#mathematics-behind-models)
- [Evaluation Metrics](#evaluation-metrics)
- [Results and Observations](#results-and-observations)
- [Conclusion](#conclusion)

## Project Overview

In this milestone, we built and compared four machine learning models for binary classification to predict stroke occurrence based on various health indicators. Our goal was to determine which model best predicts stroke risk, based on accuracy and error rates, and to understand why certain models perform better than others.

## Models Used

1. **Linear Regression**: A regression model that tries to predict a continuous target variable. Not optimized for binary classification.
   
2. **Lasso Regression**: A regularized version of Linear Regression that penalizes absolute coefficients, often used for feature selection.
   
3. **Ridge Regression**: Another regularized form of Linear Regression, which penalizes the square of coefficients, often stabilizing the model by preventing large weights.

4. **Logistic Regression**: A classification model designed to predict binary outcomes, making it well-suited for this task.

## Mathematics Behind Models

### Linear, Lasso, and Ridge Regression
- **Linear Regression**: Predicts the output by finding a linear relationship between input variables and the target. It uses the least squares method to minimize the error.
  
- **Lasso Regression**: Adds L1 regularization to the linear regression cost function, which can reduce some feature weights to zero, helping with feature selection.
  
- **Ridge Regression**: Adds L2 regularization to the linear regression cost function, which reduces model complexity by shrinking feature weights, reducing the risk of overfitting.

### Logistic Regression
- **Logistic Regression**: Unlike linear models, Logistic Regression uses the logistic/sigmoid function to map predicted values to probabilities. It’s ideal for binary classification, predicting the probability of a binary outcome.

## Evaluation Metrics

1. **Accuracy**: The percentage of correct predictions (useful for classification models).
2. **RMSE (Root Mean Square Error)**: The average deviation of predictions from actual values (common for regression models but less relevant in classification).

## Results and Observations

### Accuracy Comparison
| Model               | Accuracy (%) |
|---------------------|--------------|
| Linear Regression   | 9.47         |
| Lasso Regression    | 0.94         |
| Ridge Regression    | 9.47         |
| Logistic Regression | 93.84        |

**Observation**: Logistic Regression has the highest accuracy, making it the most suitable model for binary classification in this case.

### RMSE Comparison
| Model               | RMSE         |
|---------------------|--------------|
| Linear Regression   | 22.71        |
| Lasso Regression    | 23.76        |
| Ridge Regression    | 22.71        |
| Logistic Regression | 24.83        |

**Observation**: Linear and Ridge Regression have the lowest RMSE values, but they are not reliable for this classification task, as evidenced by their low accuracy.

## Conclusion

Based on the evaluations, **Logistic Regression** outperforms the other models in terms of accuracy, making it the best choice for stroke prediction in this dataset. Despite having a higher RMSE, Logistic Regression’s classification performance is more relevant, as accuracy is a better metric for evaluating classification models.
