# 📊 Customer Churn Prediction & Retention Analytics

An end-to-end **Data Science & Machine Learning project** that analyzes customer behavior and predicts customers who are at risk of churning from a telecommunications company.

---

## 📌 Project Overview

Customer churn is a major challenge for telecommunications companies because losing existing customers can negatively affect revenue and increase customer acquisition costs.

This project uses customer data to:

* Explore patterns associated with customer churn
* Identify important factors influencing churn
* Develop machine learning classification models
* Compare model performance
* Optimize the best-performing model
* Predict customer churn probability
* Segment customers according to churn risk
* Generate actionable business recommendations

The project demonstrates a complete machine learning workflow, from **data preparation and exploratory analysis to predictive modeling and business insights**.

---

## 🎯 Business Problem

The business wants to identify customers who are likely to leave the company so that proactive retention strategies can be applied.

The key question is:

> **Can customer characteristics and service information be used to predict which customers are most likely to churn?**

---

## 🛠️ Technologies Used

* **Python**
* **Jupyter Notebook**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **Scikit-learn**

---

## 🔄 Project Workflow

```text
Data Collection
      ↓
Data Cleaning
      ↓
Exploratory Data Analysis
      ↓
Feature Engineering
      ↓
Train/Test Split
      ↓
Machine Learning
      ↓
Model Evaluation
      ↓
Hyperparameter Tuning
      ↓
Customer Risk Prediction
      ↓
Business Recommendations
```

---

## 🤖 Machine Learning Models

Three classification algorithms were initially developed and compared:

1. Logistic Regression
2. Decision Tree
3. Random Forest

The Random Forest model was subsequently optimized using **GridSearchCV** to identify a stronger combination of hyperparameters.

The final model used for customer risk prediction was the **Tuned Random Forest**.

---

## 📈 Final Model Performance

The tuned Random Forest achieved the following results on the test dataset:

| Metric    |      Score |
| --------- | ---------: |
| Accuracy  | **78.89%** |
| Precision | **64.00%** |
| Recall    | **47.06%** |
| F1 Score  | **54.24%** |
| ROC-AUC   | **83.81%** |

The **83.81% ROC-AUC** indicates that the model has good ability to distinguish between customers who churn and those who remain.

---

## 📊 Key Visualizations

### Customer Churn Distribution

![Customer Churn Distribution](images/01-churn-distribution.png)

### Churn by Contract Type

![Churn by Contract](images/02-churn-by-contract.png)

### Churn by Tenure

![Churn by Tenure](images/03-churn-by-tenure.png)

### Churn by Payment Method

![Churn by Payment Method](images/04-churn-by-payment.png)

### Model Performance

![Model Performance](images/05-model-comparison.png)

### Feature Importance

![Feature Importance](images/06-feature-importance.png)

---

## 🔍 Top Predictive Features

The Random Forest model identified the following features as the strongest contributors to its predictions:

| Rank | Feature                                 | Importance |
| ---: | --------------------------------------- | ---------: |
|    1 | Tenure                                  |     20.97% |
|    2 | Total Charges                           |     13.02% |
|    3 | Monthly Charges                         |      8.95% |
|    4 | Fiber Optic Internet                    |      8.82% |
|    5 | Two-Year Contract                       |      7.69% |
|    6 | Electronic Check Payment                |      7.28% |
|    7 | Online Security                         |      4.42% |
|    8 | One-Year Contract                       |      3.70% |
|    9 | Technical Support                       |      2.73% |
|   10 | Device Protection — No Internet Service |      2.36% |

**Tenure** was the most important feature in the final Random Forest model.

---

## 🚨 Customer Risk Segmentation

The model generated churn probabilities that were converted into three customer risk categories:

| Risk Level  | Customers |
| ----------- | --------: |
| Low Risk    |     1,008 |
| Medium Risk |       319 |
| High Risk   |        80 |

This allows a business to prioritize customers based on their estimated churn risk rather than treating every customer equally.

---

## 💡 Key Business Insights

### 1. Customer Tenure Matters

Tenure was the strongest feature in the final model, indicating that the length of a customer's relationship with the company is highly relevant to churn prediction.

### 2. Contract Type Is Important

Contract-related features were among the important predictors, highlighting the potential relationship between contract commitment and customer retention.

### 3. Pricing Can Be Relevant

Monthly Charges and Total Charges ranked highly among the model's predictive features, suggesting that billing characteristics should be considered when developing retention strategies.

### 4. Service Type Matters

Fiber optic internet service appeared as one of the strongest predictive features, indicating that service characteristics may provide useful signals for identifying customers at risk.

### 5. Risk-Based Retention Can Improve Targeting

The model provides a churn probability for each customer, allowing retention teams to focus their resources on customers with higher predicted risk.

---

## 🎯 Business Recommendations

Based on the analysis, businesses could:

* Prioritize **high-risk customers** for proactive retention campaigns.
* Investigate the experience of customers with **shorter tenure**.
* Develop incentives that encourage customers to move toward **longer-term contracts**.
* Monitor customers with **higher monthly charges**.
* Investigate service-related issues among customers using **fiber optic services**.
* Use predictive churn scores to prioritize retention resources.

---

## ⚠️ Project Limitations

The model provides useful predictive insights, but several limitations should be considered:

* The dataset represents a specific telecommunications customer base and may not generalize to every company or market.
* Historical customer behavior does not guarantee future behavior.
* Feature importance indicates predictive contribution rather than causation.
* Additional information such as customer satisfaction, complaints, service quality, and customer interaction history could potentially improve future models.

---

## 📂 Project Structure

```text
Customer-Churn-Prediction/
│
├── notebooks/
│   └── customer_churn_analysis.ipynb
│
├── images/
│   ├── 01-churn-distribution.png
│   ├── 02-churn-by-contract.png
│   ├── 03-churn-by-tenure.png
│   ├── 04-churn-by-payment.png
│   ├── 05-model-comparison.png
│   └── 06-feature-importance.png
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 🚀 Future Improvements

Future versions of the project could explore:

* XGBoost and other advanced ensemble models
* SMOTE and other approaches to address class imbalance
* Cross-validation and threshold optimization
* Explainable AI techniques such as SHAP
* Deployment using Flask or Streamlit
* Integration with a real-time customer analytics dashboard
* Automated churn monitoring

---

## 👨‍💻 Author

**Adekunle Emmanuel Akorede**

Data Analyst | Data Science & Machine Learning Enthusiast

[GitHub](https://github.com/akoredeadekunle)
