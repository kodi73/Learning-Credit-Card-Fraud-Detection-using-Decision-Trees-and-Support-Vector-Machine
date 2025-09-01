# Credit Card Fraud Detection

This project aims to detect fraudulent credit card transactions using machine learning techniques. The dataset used in this project is the "Credit Card Fraud Detection" dataset from Kaggle.

## Data

The dataset contains credit card transactions, with features anonymized for privacy. The target variable `Class` indicates whether a transaction is fraudulent (1) or not (0). The dataset is highly imbalanced, with a very small percentage of fraudulent transactions. The dataset can be found here:
https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

## Methodology

The project follows these steps:

1. **Data Loading and Exploration**: Load the dataset and analyze its characteristics, including the distribution of the target variable.
2. **Data Preprocessing**: Standardize and normalize the features to prepare the data for machine learning models.
3. **Model Training**: Train two different models, a Decision Tree Classifier and a Linear Support Vector Machine (SVM), to classify transactions as fraudulent or legitimate. The models are trained on a split of the data, with a test set held out for evaluation. Class weights are used to address the data imbalance during training.
4. **Model Evaluation**: Evaluate the performance of the trained models using the ROC-AUC score, a suitable metric for imbalanced classification problems.

## Results

The trained models achieved the following ROC-AUC scores on the test set:

- Decision Tree Classifier: 98.936
- Linear SVM: 97.564

These results indicate that both models perform well in distinguishing between fraudulent and legitimate transactions, with the Linear SVM showing slightly better performance.

## Requirements

The following libraries are required to run the notebook:

- pandas
- scikit-learn
- matplotlib

You can install them using pip.
