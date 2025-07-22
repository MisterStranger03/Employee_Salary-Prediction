# Employee Salary Prediction

This project builds a machine‑learning pipeline to predict whether an employee’s salary falls above or below a specified threshold. Using demographic and job‑related features, the model helps organizations make data‑driven compensation decisions.

---

## 📋 Table of Contents

1. [Problem Statement](#problem-statement)  
2. [System Requirements & Technologies](#system-requirements--technologies)  
3. [Algorithm & Deployment](#algorithm--deployment)  
4. [Results](#results)  
5. [Conclusion](#conclusion)  

---

## 📝 Problem Statement

- This project aims to predict whether an employee’s salary falls above or below a specific threshold based on various personal and job-related features.  
- By analyzing demographic data, education level, work experience, and occupational attributes, we intend to uncover patterns that drive higher compensation.  
- The predictive model will assist organizations in making data-driven decisions for payroll planning, talent acquisition, and retention strategies.  
- Accurate salary forecasting enables HR departments to identify and address potential pay gaps and ensure equitable compensation.  
- The outcome will offer actionable insights into the key factors influencing salary distribution across different employee segments.  

---

## ⚙️ System Requirements & Technologies

### System Requirements
- **OS:** Windows 10, macOS, or Linux  
- **Python:** 3.8 or higher  
- **Memory:** ≥ 8 GB RAM  
- **Storage:** ≥ 200 MB free space  
- **Internet:** Required for initial setup and deployment  

### Libraries & Tools
- **Data Processing:** pandas, numpy  
- **Machine Learning:** scikit-learn  
- **Visualization:** matplotlib  
- **Web Framework & UI:** Streamlit  
- **Model Persistence:** joblib  
- **Dev Environment:** Jupyter Notebook or VS Code  

---

## 🚀 Algorithm & Deployment

1. **Data Acquisition**  
   - Load `adult 3.csv` into a Pandas DataFrame.  
   - Verify integrity: row count, column names, types.  

2. **Data Cleaning & Preprocessing**  
   - Handle missing values (drop/impute).  
   - Remove duplicates.  
   - Encode categorical variables (One‑Hot or Label Encoding).  
   - Scale numeric features with `StandardScaler`.  

3. **Exploratory Data Analysis (EDA)**  
   - Compute summary statistics.  
   - Visualize feature distributions and correlations.  
   - Identify patterns/anomalies.  

4. **Feature Engineering & Selection**  
   - Derive new features (e.g., yearly work hours).  
   - Select relevant predictors via RFE or feature‑importance.  

5. **Model Development**  
   - Split data: 80% train / 20% test.  
   - Build pipelines for:  
     - Logistic Regression  
     - Random Forest  
     - Gradient Boosting  
     - K‑Nearest Neighbors  
     - Support Vector Machine  
   - Train each pipeline on the training set.  

6. **Model Evaluation & Selection**  
   - Evaluate on test set: accuracy, precision, recall, F1‑score, ROC‑AUC.  
   - Compare results in tables and bar charts.  
   - Perform cross‑validation to confirm stability.  

7. **Deployment**  
   - Save best model with `joblib`.  
   - Develop a Streamlit app:  
     - Input widgets for all features.  
     - “Predict” button loads model and shows class & probability.  
   - Test locally (`streamlit run app.py`).  
   - (Optional) Deploy to Streamlit Community Cloud, Heroku, or AWS.  

---

## 📈 Results

- **Best Model:** Random Forest Classifier  
- **Performance:**  
  - **Accuracy:** 85%  
  - **Precision:** 0.83  
  - **Recall:** 0.82  
  - **F1‑Score:** 0.82  
- **Key Insights:** Education level, hours‑per‑week, and occupation are the strongest predictors.

---

## 🏁 Conclusion

- The Random Forest model exhibited robust performance (≈85% accuracy, 0.82 F1‑score), validating the chosen approach.  
- Education, work hours, and occupation consistently emerged as the top factors influencing salary class.  
- Challenges included handling class imbalance and optimizing categorical encodings to avoid overfitting.  
- Rigorous preprocessing (imputation, scaling) was crucial for model stability.  
- The combined ML pipeline with a Streamlit UI delivers a practical, user‑friendly salary prediction tool.

---

