# Credit-Card-Fraud-Detection

This project focuses on detecting fraudulent credit card transactions using machine learning techniques.

## Project Overview
The dataset used contains anonymized credit card transaction data, where the `Class` column indicates whether a transaction is fraudulent (1) or legitimate (0). Due to the highly imbalanced nature of the dataset (very few fraudulent transactions), two main strategies were employed:

1.  **Undersampling**: Reducing the number of legitimate transactions to match the number of fraudulent transactions.
2.  **Oversampling (SMOTE)**: Generating synthetic samples for the minority class (fraudulent transactions) to balance the dataset.

## Methodology
Both approaches involved:
- Data cleaning (removing duplicates, dropping irrelevant features).
- Splitting data into training and testing sets.
- Scaling numerical features using `StandardScaler`.
- Training a Logistic Regression model.
- Evaluating the model's performance using accuracy score.

## Results
- **Undersampling Model Accuracy**: 93.68%
- **Oversampling Model Accuracy**: 95.69%

This demonstrates that addressing class imbalance is crucial for building effective fraud detection models, with oversampling (SMOTE) yielding better performance in this particular case.
