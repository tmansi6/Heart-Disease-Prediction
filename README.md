# Heart Disease Prediction

## Overview

A supervised machine-learning project comparing Logistic Regression and Random Forest for predicting the presence of heart disease from demographic, clinical, and diagnostic characteristics.

The project focuses on the trade-off between model interpretability and predictive performance in a binary classification setting.

## Research Question

How effectively can Logistic Regression and Random Forest predict the presence of heart disease, and which model provides the stronger balance of robustness, accuracy, and interpretability?

## Dataset

The dataset contains clinical and demographic variables including:

- Age
- Sex
- Chest pain type
- Resting blood pressure
- Cholesterol
- Fasting blood sugar
- Resting ECG
- Maximum heart rate achieved
- Exercise-induced angina
- Oldpeak
- ST slope

**Target:** Binary heart-disease outcome.

## Workflow

1. Load and inspect the dataset.
2. Check data types and missing values.
3. Perform exploratory data analysis.
4. Examine distributions and relationships.
5. Assess target-class balance.
6. Encode categorical variables.
7. Scale numerical variables where required.
8. Split data into training and test sets.
9. Train Logistic Regression.
10. Train Random Forest.
11. Evaluate both models.
12. Compare performance and interpret practical implications.

## Models

### Logistic Regression

Provides an interpretable baseline for binary classification and makes it easier to understand the direction and relative contribution of predictors.

### Random Forest

Captures non-linear relationships and interactions between features and provides stronger predictive performance in this analysis.

## Results

| Model | Test Accuracy |
|---|---:|
| Logistic Regression | 84.24% |
| Random Forest | 87.00% |

Random Forest achieved the higher reported test accuracy.

The analysis also reports stronger recall and F1 performance for Random Forest, particularly for the positive class.

Random Forest achieved 100% training accuracy, which was identified as a possible indication of overfitting, although test performance remained strong.

## Key Insights

- Random Forest performed better overall on the reported test metrics.
- Logistic Regression remains valuable when interpretability and computational efficiency are priorities.
- Random Forest is better suited to capturing non-linear feature interactions.
- Model performance should be interpreted carefully because the dataset is relatively small.

## Ethical Considerations

Because the project concerns healthcare prediction, important considerations include:

- Patient privacy
- Dataset bias
- Representation of demographic groups
- Algorithmic accountability
- Risk of over-reliance on automated predictions
- Consequences of false positives and false negatives

This project should be treated as an analytical demonstration rather than a clinical diagnostic system.

## Limitations

The dataset is relatively small, and model performance may not generalise to broader or more diverse patient populations.

Further validation on larger and more representative datasets would be required before real-world clinical use.

## Tools

- Python
- pandas
- NumPy
- matplotlib
- seaborn
- scikit-learn
- Logistic Regression
- Random Forest

## Conclusion

Random Forest produced the strongest reported predictive performance, while Logistic Regression offered greater interpretability.

The comparison demonstrates the importance of evaluating both predictive performance and practical model characteristics when selecting a classification algorithm.
