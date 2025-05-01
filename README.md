# Real-Time Credit Card Fraud Detection

## 🎯 Problem Statement:
The goal of this project is to detect fraudulent credit card transactions in real-time. With the rise in credit card fraud, it is crucial for financial institutions to identify fraudulent transactions as quickly as possible to prevent financial losses and protect customers.

## 🛠️ Solution Approach:
We applied a combination of data preprocessing techniques, synthetic data generation using SMOTE (Synthetic Minority Over-sampling Technique), and various supervised machine learning models to classify transactions as either fraud or non-fraud.

### Data Preprocessing:
- Data cleaning and handling of missing values
- Feature scaling and normalization
- SMOTE for handling class imbalance by oversampling the minority class (fraudulent transactions)

### Models Used:
1. **Logistic Regression**: A baseline model for binary classification.
2. **Random Forest**: An ensemble learning model which performed best among all.
3. **XGBoost**: A gradient boosting algorithm.

### Model Evaluation Metrics:
- **F1-Score**: The F1-Score was chosen as the primary evaluation metric due to the class imbalance (fraudulent transactions are much less frequent than non-fraudulent ones).

| Model              | F1-Score (Class 1 - Fraud) |
|--------------------|----------------------------|
| Logistic Regression | 0.1183                     |
| Random Forest       | 0.8269 ✅                   |
| XGBoost             | 0.3930                     |

### Final Model:
- **Best Performing Model**: Random Forest
- **Saved Model**: `best_model.pkl` (Ready for deployment)

## 📈 Performance:
The Random Forest model achieved the best F1-Score of **0.8269** for detecting fraudulent transactions, making it the optimal choice for real-time fraud detection.

## ⚙️ How to Use:
1. Clone this repository:
   ```bash
   git clone https://github.com/your_username/fraud-detection.git
   cd fraud-detection
