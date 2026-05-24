# Employee Attrition Prediction (Machine Learning Project)

## 📌 Project Overview
This project aims to predict employee attrition (whether an employee will leave or stay) using machine learning models. The goal is to help organizations identify employees at risk of leaving and support better HR decision-making.

---

## 📊 Dataset Description
The dataset contains 600 employee records with the following features:

- EmployeeID
- Age
- MonthlyIncome
- YearsAtCompany
- JobSatisfaction
- WorkLifeBalance
- OverTime
- Department
- JobRole
- Attrition (Target Variable)

---

## 🧹 Data Cleaning
The following data preprocessing steps were performed:

- Handled missing values in MonthlyIncome and JobRole
- Converted MonthlyIncome from string to numeric
- Encoded categorical variables (Department, JobRole)
- Converted OverTime into numerical format
- Removed unnecessary columns like EmployeeID

---

## 🧠 Feature Engineering
To improve model performance, new features were created:

- IncomePerYear: Monthly income adjusted by experience
- OverTime_Risk: Converted overtime into binary risk indicator
- Stress_Level: Combined JobSatisfaction and WorkLifeBalance into a stress score

---

## 🤖 Models Used
The following machine learning models were trained and evaluated:

- Logistic Regression
- Random Forest Classifier
- SMOTE + Random Forest (to handle class imbalance)

---

## ⚖️ Handling Class Imbalance
Since the dataset was imbalanced, SMOTE (Synthetic Minority Oversampling Technique) was applied to improve model learning on minority class (employees who leave).

---

## 📈 Results Summary

- Logistic Regression struggled to detect employee attrition.
- Random Forest performed better but still missed many attrition cases.
- SMOTE improved balance slightly but model still had difficulty detecting class 1 (attrition).

Overall, the dataset showed weak predictive signals for employee attrition.

---

## 🧠 Key Insights

- Employee attrition is difficult to predict with basic HR features alone.
- Class imbalance significantly affects model performance.
- Feature engineering improves performance but is not always sufficient.
- More advanced models or richer data may be needed for better predictions.

---

## 🚀 Future Improvements

- Use advanced models like XGBoost or LightGBM
- Add more HR features (performance rating, promotions, salary growth)
- Perform hyperparameter tuning
- Improve feature engineering

---

## 🛠️ Libraries Used

- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- imbalanced-learn

---

## 📂 Project Structure
