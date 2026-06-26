# Telecom Customer Churn Prediction using Machine Learning

## 📊 Project Overview

Customer churn is one of the biggest challenges faced by telecom companies. Predicting customers who are likely to discontinue a service helps businesses take proactive retention measures.

This project develops an end-to-end Machine Learning pipeline to predict customer churn using customer demographics, subscription details, and service usage patterns. It also performs customer segmentation using K-Means Clustering to identify different customer groups and support business decision-making.

---

## 🎯 Objectives

* Predict customer churn using Machine Learning.
* Handle class imbalance using SMOTE.
* Optimize model performance using RandomizedSearchCV.
* Compare multiple Machine Learning models.
* Evaluate model performance using multiple metrics.
* Segment customers using K-Means Clustering.
* Generate business insights for customer retention.

---

## 📂 Dataset

**Dataset:** Telco Customer Churn Dataset

* Total Customers: **7,043**
* Original Features: **33**
* Features after preprocessing: **30**
* Target Variable: **Churn Value**

---

## 🛠 Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Imbalanced-learn

---

## Project Workflow

### 1. Data Preprocessing

* Data cleaning
* Missing value handling
* Feature encoding
* Train-test split

### 2. Exploratory Data Analysis

* Customer tenure analysis
* Monthly charges analysis
* Contract type analysis
* Internet service analysis
* Payment method analysis
* Correlation heatmap

### 3. Handling Class Imbalance

* SMOTE (Synthetic Minority Oversampling Technique)

### 4. Machine Learning Models

* Logistic Regression
* Decision Tree
* Random Forest
* Support Vector Machine (SVM)

### 5. Hyperparameter Tuning

Random Forest was optimized using **RandomizedSearchCV** by tuning:

* Number of trees
* Maximum depth
* Minimum samples split
* Minimum samples leaf
* Maximum features

### 6. Model Evaluation

Evaluation metrics:

* Accuracy
* Precision
* Recall
* F1 Score
* Confusion Matrix
* ROC Curve
* Precision-Recall Curve
* Cross Validation

### 7. Feature Importance

Permutation Feature Importance was used to identify the most influential features affecting customer churn.

### 8. Customer Segmentation

Customer segmentation was performed using **K-Means Clustering**.

The Elbow Method was used to determine the optimal number of clusters.

Identified customer groups:

* Highest Churn Risk Customers
* Moderate Churn Risk Customers
* Loyal Customers

---

## 📈 Model Performance

**Best Model:** Random Forest (RandomizedSearchCV)

| Metric    | Score |
| --------- | ----: |
| Accuracy  |  ~79% |
| Precision |  ~62% |
| Recall    |  ~67% |
| F1 Score  |  ~65% |

---

## 💡 Key Business Insights

* Customers with shorter tenure are more likely to churn.
* Fiber Optic users exhibit a higher churn rate.
* Month-to-Month contracts have the highest churn probability.
* Customers without Tech Support are more likely to churn.
* Customer segmentation identified High Risk, Moderate Risk, and Loyal customer groups for targeted retention strategies.

---

## Repository Structure

```text
Telecom-Customer-Churn-Prediction/
│
├── Telecom_Customer_Churn_Prediction.ipynb
├── Telco_customer_churn.xlsx
├── README.md
├── requirements.txt
├── roc_curve.png
├── feature_importance.png
├── confusion_matrix.png
├── customer_segmentation.png
├── elbow_method.png
└── precision_recall_curve.png
```

---

## Future Improvements

* Deploy using Streamlit
* Build a real-time prediction application
* Explore XGBoost and LightGBM
* Add model explainability using SHAP

---

## How to Run

1. Clone this repository.
2. Install the required libraries.

```bash
pip install -r requirements.txt
```

3. Open the notebook.

```bash
jupyter notebook Telecom_Customer_Churn_Prediction.ipynb
```

4. Run all cells sequentially.

---

## Author

**Khushi Singh**
