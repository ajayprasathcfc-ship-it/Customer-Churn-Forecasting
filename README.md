## Project Workflow

```text
1. Data Collection
2. Data Cleaning
3. Data Preprocessing
4. Feature Engineering
5. Feature Scaling
6. Handling Class Imbalance using SMOTE
7. Model Training
8. Hyperparameter Tuning
9. Model Evaluation
10. Business Insights Generation
```

---

## Exploratory Data Analysis (EDA)

EDA was performed to identify important customer behavior patterns and churn trends.

### Key Analysis Performed

- Churn distribution analysis
- Tenure vs churn comparison
- Usage frequency analysis
- Payment delay analysis
- Support call frequency analysis
- Correlation heatmap analysis

### Visualizations Used

- Count plots
- Box plots
- Heatmaps
- Confusion matrix
- Feature importance plots

These visualizations helped identify the major factors influencing customer churn.

---

## Models Used

The following machine learning models were implemented and compared:

| Model | Purpose |
|---|---|
| K-Nearest Neighbors (KNN) | Distance-based classification |
| Random Forest | Ensemble learning and feature importance |
| XGBoost | Gradient boosting for optimized prediction |

---

## Final Model Selection

The **Random Forest model** was selected as the final model because it achieved the best balance between:

- Accuracy
- Precision
- Recall
- F1-score
- ROC-AUC score

compared to KNN and XGBoost models.

### Final Random Forest Performance

| Metric    | Score |
|------------|--------|
| Accuracy   | 84%    |
| Precision  | 82%    |
| Recall     | 78%    |
| F1-score   | 80%    |
| ROC-AUC    | 0.87   |

---

## Business Value of the Project

This project helps businesses:

- Predict customer churn proactively
- Improve customer retention strategies
- Reduce revenue loss
- Identify high-risk customers
- Support data-driven business decisions

---

## Conclusion

This project demonstrates how machine learning techniques can be applied to predict customer churn and improve customer retention strategies.

By combining:

- Data preprocessing
- Feature engineering
- SMOTE
- Exploratory data analysis
- Machine learning models

the system effectively identifies customers likely to churn and provides actionable business insights for businesses.
