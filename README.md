# Credit Card Fraud Detection 

## Problem Statement 

The goal of this project is to predict fraudulent credit card transactions using machine learning models. 

We analyze customer-level data collected through a research collaboration between Worldline and the Machine Learning Group. The dataset, sourced from the [Kaggle Website](https://www.kaggle.com/mlg-ulb/creditcardfraud), contains 284,807 transactions, of which 492 are fraudulent. Given the highly imbalanced nature of the dataset, appropriate handling techniques are required before model building.

---

## Business Problem Overview

For banks, retaining high-value customers is a top priority. However, banking fraud poses a significant challenge, leading to substantial financial losses and eroding trust and credibility. 

According to the [Nilson Report](https://nilsonreport.com/upload/content_promo/The_Nilson_Report_Issue_1164.pdf), banking frauds were projected to reach $30 billion globally by 2020. The increasing adoption of digital payment channels has further amplified the risk of fraudulent transactions, with fraudsters continuously innovating new techniques.

Credit card fraud detection is no longer optional but a necessity for banks to implement proactive monitoring and fraud prevention mechanisms. Machine learning is pivotal in this effort, helping institutions reduce manual reviews, costly chargebacks, false positives, and denial of legitimate transactions.

---

## Understanding and Defining Fraud

Credit card fraud involves unauthorized actions to obtain financial information for personal gain. Common types of fraud include:

- **Skimming:** Duplicating card information from the magnetic strip.
- **Card Manipulation/Alteration:** Altering genuine cards.
- **Counterfeit Card Creation:** Producing fake cards.
- **Stolen/Lost Cards:** Using cards without the owner's consent.
- **Fraudulent Telemarketing:** Scamming individuals via deceptive calls.

---

## Data Dictionary

The dataset, available [here](https://www.kaggle.com/mlg-ulb/creditcardfraud), contains transactions made by European cardholders over two days in September 2013. 

### Key Characteristics:
- **Total Transactions:** 284,807
- **Fraudulent Transactions:** 492 (0.172% of the total)
- **Features:** 
  - `Time`: Seconds elapsed between the first transaction and subsequent transactions.
  - `Amount`: Transaction amount.
  - `Class`: 1 for fraud, 0 otherwise.
  - `V1` to `V28`: Principal components derived using PCA for confidentiality.

---

## Project Pipeline

### 1. **Data Understanding**
   - Load and explore the dataset.
   - Identify key features for model building.

### 2. **Exploratory Data Analysis (EDA)**
   - Perform univariate and bivariate analyses.
   - Check for skewness and apply transformations if necessary.
   - Evaluate the distribution of features.

### 3. **Train/Test Split**
   - Split the dataset into training and testing sets.
   - Use k-fold cross-validation to ensure minority class representation in test folds.

### 4. **Model Building & Hyperparameter Tuning**
   - Experiment with various machine learning models.
   - Use techniques like oversampling, undersampling, or SMOTE to address class imbalance.
   - Optimize model hyperparameters for better performance.

### 5. **Model Evaluation**
   - Evaluate models using metrics suitable for imbalanced datasets (e.g., precision, recall, F1-score, ROC-AUC).
   - Prioritize identifying fraudulent transactions over non-fraudulent ones to align with business goals.

---

## Conclusion

This project aims to demonstrate the application of machine learning in solving a critical real-world problem. By leveraging advanced techniques, we can improve fraud detection accuracy, reduce financial losses, and enhance customer trust.

---
