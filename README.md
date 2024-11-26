# Machine Learning Models for Tumor Classification and Lung Cancer Prediction

This project applies machine learning models to classify tumor types and predict cancer outcomes, specifically for lung cancer, using gene expression data. The models used include Random Forest, C5.0 Decision Trees, Support Vector Machines (SVM), and Artificial Neural Networks (ANN). The models undergo hyperparameter tuning, cross-validation, and performance evaluation.

## Table of Contents
1. [Data Preprocessing](#data-preprocessing)
2. [Models Applied](#models-applied)
3. [Model Evaluation and Comparison](#model-evaluation-and-comparison)
4. [Final Model and Evaluation](#final-model-and-evaluation)
5. [Conclusion](#conclusion)
6. [References](#references)

## 1. Data Preprocessing
- **Training and Validation Split**: The dataset is divided into training and validation sets for model training and evaluation.
- **Feature Scaling**: Data is standardized to ensure fair model training.
- **Other Preprocessing**: Includes data cleaning, transformation, balancing, and dimensionality reduction to improve model performance.

## 2. Models Applied

### Random Forest (RF)
Random Forest is effective for handling diverse datasets and preventing overfitting. The key model (`rf_model6`) showed high performance with an out-of-bag (OOB) error rate of 0.14%.

### C5.0 Decision Trees
C5.0 is used for its interpretability, achieving 71.34% accuracy in tumor classification.

### Support Vector Machines (SVM)
SVM is applied to improve classification performance, with high accuracy of 90.45%.

### Artificial Neural Networks (ANN)
The ANN model showed significant improvement after tuning, achieving 99.73% accuracy after 5-fold cross-validation and hyperparameter optimization.

## 3. Model Evaluation and Comparison
- **Metrics**: Models were evaluated using accuracy, precision, recall, F1-score, and ROC curves.
- **SVM and ANN Models**: Showed superior performance compared to Random Forest and C5.0 models. ANN demonstrated potential overfitting, which was mitigated through tuning.
- **Ensemble Model**: A heterogeneous ensemble model combining all four models (RF, C5.0, SVM, ANN) outperformed individual models. It uses a majority voting mechanism for predictions, showing robustness and generalization across datasets.

## 4. Final Model and Evaluation
The ensemble model achieved the following performance metrics on the testing set:
- **Accuracy**: 89.2%
- **Precision**: 77.6%
- **Recall**: 100%
- **Specificity**: 83%
- **F1 Score**: 87.3%

These results indicate strong performance and generalizability across multiple performance metrics.

## 5. Conclusion
This analysis demonstrates the utility of machine learning models in cancer classification and prediction. The ensemble model provides the most reliable predictions across multiple performance metrics. Future work will focus on improving ANN stability and exploring other cancer types.
