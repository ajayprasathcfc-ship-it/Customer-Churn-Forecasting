# Customer-Churn-Forecasting
# Customer Churn Forecasting using K-Nearest Neighbors (KNN)

## Project Overview

Customer churn refers to the situation where customers stop using a company's product or service. Predicting churn is important for businesses because retaining existing customers is often more cost-effective than acquiring new ones.

This project develops a **Customer Churn Forecasting system** using the **K-Nearest Neighbors (KNN)** machine learning algorithm. The goal is to identify customers who are likely to leave a service based on their behavioral and demographic information.

The project includes **data preprocessing, exploratory data analysis, feature scaling, model training, and evaluation**. Additionally, the **SMOTE (Synthetic Minority Oversampling Technique)** method is used to address class imbalance in the dataset.

---

## Dataset Description

The dataset contains customer information related to service usage and interaction history. Each row represents a customer and the target variable indicates whether the customer churned or not.

### Features Used

* **CustomerID** – Unique identifier for each customer
* **Age** – Age of the customer
* **Gender** – Gender of the customer
* **Tenure** – Number of months the customer has used the service
* **Usage Frequency** – Frequency of service usage
* **Support Calls** – Number of customer support interactions
* **Payment Delay** – Delay in payment by the customer
* **Subscription Type** – Type of subscription plan
* **Contract Length** – Duration of the service contract
* **Total Spend** – Total amount spent by the customer
* **Last Interaction** – Most recent customer interaction
* **Churn** – Target variable (1 = Churn, 0 = No Churn)

---

## Data Preprocessing

The dataset was prepared before model training through several preprocessing steps:

1. **Handling Missing Values**
   Missing values were removed to ensure data consistency.

2. **Encoding Categorical Variables**
   Categorical features such as subscription type and contract length were converted into numerical form using one-hot encoding.

3. **Feature Scaling**
   Since KNN relies on distance calculations, all numerical features were standardized using the **StandardScaler** technique.

4. **Train-Test Split**
   The dataset was divided into training and validation sets to evaluate model performance.

---

## Handling Class Imbalance

Customer churn datasets are often imbalanced, meaning one class appears more frequently than the other. To solve this problem, **SMOTE (Synthetic Minority Oversampling Technique)** was applied to the training data.

SMOTE generates synthetic samples of the minority class by interpolating between existing samples. This helps the model learn better decision boundaries and improves classification performance.

---

## Machine Learning Model

### K-Nearest Neighbors (KNN)

KNN is a supervised machine learning algorithm used for classification problems. It works by finding the **k nearest data points** in the dataset and assigning the majority class among them.

Steps followed in the KNN algorithm:

1. Calculate the distance between the new data point and all training data points.
2. Select the **k nearest neighbors**.
3. Assign the class based on the majority vote among neighbors.

Feature scaling is important for KNN because it uses distance-based calculations.

---

## Model Evaluation

The performance of the model was evaluated using several classification metrics.

### Evaluation Metrics

* **Accuracy** – Overall correctness of the model
* **Precision** – Correctly predicted churn customers out of all predicted churn customers
* **Recall** – Ability of the model to detect actual churn customers
* **F1 Score** – Harmonic mean of precision and recall
* **Confusion Matrix** – Visualization of prediction performance

These metrics help measure how effectively the model identifies customers likely to churn.

---

## Tools and Libraries Used

The project was implemented using the following Python libraries:

* **Pandas** – Data manipulation and preprocessing
* **NumPy** – Numerical operations
* **Matplotlib** – Data visualization
* **Seaborn** – Statistical visualization
* **Scikit-learn** – Machine learning algorithms and evaluation metrics
* **Imbalanced-learn** – SMOTE for handling class imbalance

---

## Key Insights

The model analysis shows that several factors strongly influence customer churn:

* Customers with **low usage frequency** are more likely to leave.
* Customers with **short tenure** show higher churn rates.
* Frequent **support calls** may indicate dissatisfaction with the service.
* **Payment delays** can signal financial or service-related dissatisfaction.

These factors help businesses identify customers who are at risk of leaving.

---

## Business Recommendations

Based on the churn prediction results, businesses can take proactive steps to improve retention:

1. **Target At-Risk Customers**
   Offer personalized discounts or retention campaigns to customers predicted to churn.

2. **Improve Customer Support**
   Reduce churn caused by unresolved service issues.

3. **Increase Customer Engagement**
   Encourage low-usage customers to inter
