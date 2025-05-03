# Fraudulent Credit Card Transaction Prediction

## Problem Statement
The goal of this project is to predict fraudulent credit card transactions using machine learning models. This involves analyzing customer-level data collected during a research collaboration between Worldline and the Machine Learning Group.

The dataset, sourced from Kaggle, contains 284,807 transactions, of which 492 are fraudulent. Due to the highly imbalanced nature of the dataset, special handling is required before building models.

---

## Business Problem Overview
For banks, retaining high-value customers is a top priority. However, banking fraud poses a significant threat to this goal, leading to financial losses, reduced trust, and damaged credibility. 

According to the Nilson Report, banking frauds were estimated to account for $30 billion worldwide by 2020. With the rise of digital payment channels, fraudulent transactions are increasing in both volume and sophistication. 

Machine learning has become essential for banks to implement proactive fraud detection and prevention mechanisms. It helps reduce manual reviews, costly chargebacks, and denials of legitimate transactions.

---

## Understanding and Defining Fraud
Credit card fraud refers to any dishonest act to obtain financial information without proper authorization. Common methods include:
- Skimming: Duplicating information from the card's magnetic strip.
- Manipulation or alteration of genuine cards.
- Creation of counterfeit cards.
- Stealing or losing credit cards.
- Fraudulent telemarketing.

---

## Data Dictionary
The dataset includes credit card transactions made by European cardholders over two days in September 2013. Key details:
- **Total transactions**: 284,807
- **Fraudulent transactions**: 492 (0.172% of total)
- **Features**:
  - `Time`: Seconds elapsed between the first transaction and subsequent transactions.
  - `Amount`: Transaction amount.
  - `Class`: Fraud label (1 for fraud, 0 for non-fraud).
  - `V1` to `V28`: Principal components obtained using PCA for confidentiality.

The dataset is highly imbalanced and has been preprocessed using PCA.

---

## Project Pipeline
The project follows these steps:

1. **Data Understanding**:
   - Load and explore the dataset.
   - Identify relevant features for model building.

2. **Exploratory Data Analysis (EDA)**:
   - Perform univariate and bivariate analyses.
   - Address skewness in the data, if necessary.

3. **Train/Test Split**:
   - Split the data into training and testing sets.
   - Use k-fold cross-validation to ensure the minority class is well-represented.

4. **Model Building and Hyperparameter Tuning**:
   - Experiment with different machine learning models.
   - Fine-tune hyperparameters for optimal performance.
   - Explore sampling techniques to handle class imbalance.

5. **Model Evaluation**:
   - Use appropriate evaluation metrics to assess model performance.
   - Focus on accurately identifying fraudulent transactions.

---

## Dataset
The dataset can be downloaded from [Kaggle](https://www.kaggle.com/datasets).

---

## Evaluation Metrics
Given the imbalanced nature of the dataset, the focus is on accurately identifying fraudulent transactions. Metrics such as precision, recall, F1-score, and AUC-ROC are recommended for evaluation.

---

## Conclusion
This project aims to leverage machine learning to address the critical issue of credit card fraud detection, providing banks with a robust solution to safeguard their customers and assets.