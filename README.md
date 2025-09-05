# 💳 Credit Card Fraud Detection using Machine Learning

This project detects fraudulent credit card transactions using the **Random Forest** algorithm.  
The dataset is highly imbalanced, with fraud cases making up less than 0.2% of total transactions.

---

## 📂 Dataset

**Source:** [Kaggle - Credit Card Fraud Detection](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)  

**Features:**
- `V1`–`V28`: PCA-transformed numerical features  
- `Time`: Seconds elapsed between this transaction and the first transaction in the dataset  
- `Amount`: Transaction amount  
- **Target:** `Class` → `0 = Legitimate`, `1 = Fraudulent`  

---

## ⚙️ Steps Performed

### Data Preprocessing
- Handled **class imbalance** using Random Forest with class weights.  
- Normalized numerical features (`Amount`, `Time`).  
- Train-test split (80/20).  

### Exploratory Data Analysis (EDA)
- Distribution plots of `Amount`, `Time`, and PCA features.  
- Fraud vs. Non-Fraud transaction count visualization.  
- Correlation heatmap to study feature relationships.  

### Model Training
- **Random Forest Classifier** with hyperparameter tuning.  
- Compared with baseline models (e.g., Logistic Regression).  

### Model Evaluation
- Accuracy score  
- Precision, Recall, F1-score  
- Confusion matrix  
- ROC-AUC curve  

---

## 📊 Results

**Classification Report:**

| Class       | Precision | Recall | F1-Score | Support |
|-------------|-----------|--------|----------|---------|
| 0 (Legit)   | 0.9998    | 0.9998 | 0.9998   | 28,326  |
| 1 (Fraud)   | 0.8723    | 0.8723 | 0.8723   | 47      |

**Overall Metrics:**
- **Accuracy:** 99.96%  
- **Macro Avg F1-Score:** 93.61%  
- **Weighted Avg F1-Score:** 99.96%  
- **ROC-AUC:** 0.975  

✅ **Best Model:** Random Forest – achieved near-perfect performance for legitimate transactions while maintaining strong precision and recall for fraud cases.  

---

## 📌 Insights

- Fraudulent transactions are **extremely rare**, requiring class imbalance handling.  
- **Precision and Recall** are more important than accuracy in fraud detection.  
- Random Forest outperformed baseline models, balancing fraud detection without excessive false positives.  
- PCA-transformed features limit interpretability but still capture meaningful variance for classification.  

---

## 🚀 Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/credit-card-fraud-detection.git
   cd credit-card-fraud-detection
