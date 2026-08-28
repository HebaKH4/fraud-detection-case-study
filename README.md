# Fraud Detection Case Study

## Objective
Build a predictive model to identify fraudulent credit card transactions from transaction data, and translate the results into business recommendations.

## Dataset
~594,000 transactions with features including transaction category, merchant, customer demographics, and amount. Fraud rate: 1.21%.

## Approach
1. Exploratory Data Analysis
2. Data cleaning and preprocessing
3. Feature engineering
4. Model comparison (Logistic Regression, Random Forest, XGBoost)
5. Hyperparameter tuning
6. Evaluation on held-out test set
7. Feature importance / model interpretation

## Key Results
- Best model: XGBoost (tuned)
- PR-AUC: 0.893 | AUC-ROC: 0.997 | Recall: 96.6%
- Primary drivers: transaction category (especially transportation) and merchant identity

## Repository Structure
```
├── data/              # Not included (see .gitignore) — raw dataset
├── notebooks/         # Main analysis notebook
├── outputs/           # Saved model and generated plots
├── requirements.txt   # Python dependencies
```

## How to Run
1. Create a virtual environment and install dependencies: `pip install -r requirements.txt`
2. Place the dataset in `data/`
3. Run `notebooks/fraud_detection_case_study.ipynb`
