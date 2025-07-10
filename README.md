# 💳 Credit Card Fraud Detection

A machine learning project for detecting fraudulent credit card transactions using PCA-transformed features. The dataset is heavily imbalanced and real-world, containing anonymized transaction data.

## 📦 Dataset

- Source: [Kaggle – Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
- Features:
  - 30 total columns
  - `Time`, `Amount`, `Class` (target: 1 = Fraud, 0 = Legit)
  - `V1` to `V28` are PCA components

## 📊 Exploratory Steps

- Loaded the dataset and verified that:
  - No null/missing values
  - Highly imbalanced target classes (majority are non-fraud)

## 🧪 Preprocessing

- Split data into:
  - **Legit** transactions (`Class == 0`)
  - **Fraudulent** transactions (`Class == 1`)
- Basic EDA on shape and distribution

## 🤖 Model

- **Model Used**: Logistic Regression (`sklearn`)
- **Train/Test Split**: 80% training, 20% testing
- **Evaluation Metric**: Accuracy Score

## 📁 Project Structure

├── Fraud_detection.ipynb # Jupyter notebook with all code
├── kaggle.json # Kaggle API token (not committed)
├── creditcard.csv # Dataset (downloaded via Kaggle API)
└── README.md
