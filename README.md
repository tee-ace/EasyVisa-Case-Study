# 🧠 EasyVisa Case Status Prediction

This project aims to predict the outcome of U.S. visa applications (Certified or Denied) using machine learning models, enabling automation and efficiency in reviewing visa requests.

## 📌 Project Overview

- **Context**: U.S. employers frequently sponsor foreign workers. With the growing number of visa applications, there's a need for predictive tools to support decision-making.
- **Goal**: Build a classification model that predicts visa outcomes using applicant and employer attributes.
- **Dataset**: Contains 25,480 rows with features like education, job experience, wage, continent, and region of employment.

## 🧪 Approach

- **EDA**: Analyzed feature distributions, class imbalance, and categorical breakdowns.
- **Preprocessing**: Handled encoding, wage normalization, and sampling (SMOTE and undersampling).
- **Models Used**:
  - Decision Tree
  - Random Forest
  - Bagging Classifier
  - Gradient Boosting
  - AdaBoost
  - XGBoost ✅ (best performance)
  - Stacking Classifier

- **Evaluation Metric**: F1-Score (to balance false positives and false negatives).
- **Best Model**: XGBoost (F1 = 0.816 on validation with oversampled data).

## 🔍 Key Insights

- Applicants with High School education, favorable employment regions (e.g., South, Northeast), and prior job experience were more likely to be certified.
- Wage had lower importance than expected.
- Ensemble models outperformed simple trees; XGBoost showed the most stable generalization.

## 📊 Results

| Model         | Validation F1 |
|---------------|---------------|
| Decision Tree | 0.738         |
| Random Forest | 0.755         |
| AdaBoost      | 0.808         |
| GradientBoost | 0.813         |
| **XGBoost**   | **0.816** ✅   |

## 📂 Files

- `EasyVisa_Low_Code_1.ipynb` – Main analysis notebook
- `EasyVisa.csv` – Dataset
- `presentation/` – Slides and visuals
- `models/` – (Optional) Saved models and metrics

## 🚀 Next Steps

- Deploy XGBoost model as an API for real-time visa screening.
- Automate retraining pipeline using new visa data.
- Build dashboards for visa approval probability monitoring.

## 📧 Contact

Tade Odunlami  
[LinkedIn](https://www.linkedin.com/in/your-link) | [Email](mailto:your.email@example.com)
