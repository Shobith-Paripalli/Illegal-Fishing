# Illegal Fishing Detection using Supervised Machine Learning

## Project Overview
This project focuses on developing a supervised machine learning framework to identify illegal fishing activities. The dataset consists of 8 features and contains 8,38,860 data points classified into three categories: -1, 0, 1.

## Dataset Description
The dataset includes the following features:
- **mmsi**: Maritime Mobile Service Identity
- **timestamp**: Time of data capture
- **distance from shore**: Distance of the vessel from the shore
- **distance from port**: Distance of the vessel from the nearest port
- **speed**: Speed of the vessel
- **course**: The direction in which the vessel is moving
- **latitude**: Latitude position of the vessel
- **longitude**: Longitude position of the vessel

## Exploratory Data Analysis
- **Feature Plots**:
  - Distance from shore vs Distance from port
  - Distribution of Course
- Class Distribution

## Methodology
1. **Feature Selection and Class Imbalance Handling**:
   - Addressed class imbalance using SMOTEENN (Synthetic Minority Over-sampling Technique combined with Edited Nearest Neighbors).
   - Applied feature selection to identify significant features.

2. **Classification Techniques**:
   - Implemented and evaluated various classifiers, including Logistic Regression, Decision Tree, Random Forest, Gradient Boosting, K-Nearest Neighbors, and Support Vector Machine.

3. **Performance Evaluation**:
   - Evaluated performance using Precision, Recall, and F-measure.
   - Optimized hyperparameters using GridSearchCV and RandomizedSearchCV.

## Results
### Performance Using All Features
| Classifier               | Precision | Recall | F-measure |
|--------------------------|-----------|--------|-----------|
| Logistic Regression       | 0.32      | 0.33   | 0.33      |
| Decision Tree             | 0.94      | 0.94   | 0.94      |
| Random Forest             | 0.95      | 0.93   | 0.94      |
| Gradient Boosting         | 0.90      | 0.80   | 0.85      |
| K-Nearest Neighbors       | 0.96      | 0.95   | 0.96      |
| Support Vector Machine    | 0.32      | 0.33   | 0.33      |

### Performance After Feature Selection and SMOTEENN
| Classifier               | Precision | Recall | F-measure |
|--------------------------|-----------|--------|-----------|
| Logistic Regression       | 0.32      | 0.33   | 0.33      |
| Decision Tree             | 0.76      | 0.97   | 0.84      |
| Random Forest             | 0.79      | 0.98   | 0.86      |
| Gradient Boosting         | 0.52      | 0.92   | 0.60      |
| K-Nearest Neighbors       | 0.46      | 0.80   | 0.51      |
| Support Vector Machine    | 0.92      | 0.96   | 0.94      |

## Conclusion
This study thoroughly evaluated several machine learning classifiers for identifying illegal fishing activities. The Decision Tree and Random Forest models, with hyperparameter optimization, exhibited superior performance. Applying feature selection and SMOTEENN further enhanced model precision, recall, and F-measure.

## Future Work
- Explore advanced ensemble methods.
- Apply more sophisticated feature engineering techniques.
- Expand the dataset for more robust analysis and better model generalization.
