# Credit-card-fraud-detection
A machine learning project for detecting fraudulent credit card transactions using the Random Forest algorithm. The model is trained on an imbalanced dataset and evaluated with performance metrics such as accuracy, precision, recall, and F1-score to ensure reliable fraud detection.

##  Dataset

The model uses the publicly available [Credit Card Fraud Detection dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud) from Kaggle. It contains anonymized European credit card transactions from September 2013, covering a brief two-day period. Out of **284,807** transactions, only **492** are fraudulent—making the dataset extremely imbalanced (~0.172 %) :contentReference[oaicite:0]{index=0}.

All features are numerical results of PCA, named `V1`, `V2`, ..., `V28`. The only non-transformed features are:
- `Time` – seconds elapsed since the first transaction
- `Amount` – transaction amount  
The target variable `Class` is `1` for fraud and `0` otherwise :contentReference[oaicite:1]{index=1}.
