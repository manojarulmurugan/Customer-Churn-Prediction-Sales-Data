# 🔄 Customer Churn Prediction

## 📌 Project Overview
This project is an **extension of Sales Forecasting**, focusing on predicting **customer churn** using machine learning, ECDF and Forecasting methods. By analyzing customer behavior and purchase history, we identify customers likely to stop doing business and recommend retention strategies.

---

## **🎯 Business Objectives**
✅ **Predict which customers are likely to churn**.  
✅ **Understand key factors contributing to churn**.  
✅ **Recommend targeted strategies to improve customer retention**.  

---

## **📊 Dataset**
- **Source**: Customer purchase and interaction data.
- **Size**: Includes past purchase history, frequency, and behavioral trends.
- **Key Features**:
  - **Purchase Frequency**: Number of purchases in the last X months.
  - **Time Since Last Purchase**: Days since last transaction.
  - **Revenue Contribution**: Total spending by customer.
  - **Product Category & Segmentation**.

📌 **Data Preprocessing Steps**
- **Handling missing values** with median imputation.
- **Feature scaling** using standardization.
- **Class imbalance handling** with **SMOTE oversampling**.

---

## **🛠️ Model Architectures**
### **1️⃣ Classification Models for Churn Prediction**
| Model | Accuracy | Precision | Recall |
|--------|---------|-----------|--------|
| **Logistic Regression** | 85% | 0.84 | 0.82 |
| **Random Forest** | 91% | 0.89 | 0.86 |
| **XGBoost (Best Model)** | **94.2%** | **0.92** | **0.91** |

📌 **Findings**:
- **Purchase frequency & recency are key churn indicators**.
- **XGBoost outperforms traditional models**, showing better generalization.
- **SMOTE improved recall**, ensuring churned customers are correctly classified.

---

## **🔍 Feature Importance**
![Feature Importance](reports/images/feature_importance.png)

📌 **Key Predictive Features**:
1. **Time Since Last Purchase** (High impact)
2. **Revenue Contribution** (Loyalty Indicator)
3. **Product Category Preferences** (Churn tendency varies by product type)

---

## **📈 Model Evaluation**
### **Confusion Matrix**
![Confusion Matrix](reports/images/confusion_matrix.png)

### **Precision-Recall Curve**
![PR Curve](reports/images/precision_recall.png)

📌 **Key Insights**:
- High **Recall ensures most churned customers are detected**.
- **Precision-Recall trade-off optimized using hyperparameter tuning**.

---

## **📌 Retention Strategies Based on Model Insights**
🔹 **Early Warning System**: Flag customers likely to churn based on model predictions.  
🔹 **Personalized Offers**: Provide discounts & incentives to at-risk customers.  
🔹 **Loyalty Rewards**: Encourage repeat purchases with membership benefits.  
🔹 **Automated Follow-ups**: Send reminders based on inactivity periods.  

---

## **📁 File Structure**
```plaintext
Customer_Churn_Prediction/
├── README.md
├── data/
├── notebooks/
├── reports/
├── src/
├── models/
├── results/
├── requirements.txt
└── LICENSE

