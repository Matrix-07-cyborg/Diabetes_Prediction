# 🩺 Diabetes Prediction using Logistic Regression

## 📌 Project Overview
This project uses the **Pima Indians Diabetes Dataset** to build a machine learning model that predicts whether a person has diabetes based on diagnostic measurements.  
The main focus is on **Logistic Regression**, data preprocessing, and evaluating the trade-offs between **precision and recall** by adjusting classification thresholds.

---

## ⚙️ Tech Stack
- **Programming Language:** Python  
- **Libraries:** Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn  

---

## 📂 Dataset Information
The dataset consists of **768 entries** with **9 features**:

| Feature | Description |
|---------|-------------|
| Pregnancies | Number of times pregnant |
| Glucose | Plasma glucose concentration (after 2-hour test) |
| BloodPressure | Diastolic blood pressure (mm Hg) |
| SkinThickness | Triceps skin fold thickness (mm) |
| Insulin | 2-hour serum insulin (mu U/ml) |
| BMI | Body Mass Index (kg/m²) |
| DiabetesPedigreeFunction | Genetic risk factor for diabetes |
| Age | Age in years |
| Outcome | Target variable (0 = Non-diabetic, 1 = Diabetic) |

⚠️ Note: Some features contain **zero values** (e.g., BloodPressure = 0), which are physiologically invalid and need to be treated as missing values during preprocessing.

---

## 🚀 Project Workflow
1. **Data Preprocessing**
   - Handled invalid zero values by imputation.
   - Feature scaling using `StandardScaler`.
   - Train-test split for model evaluation.

2. **Modeling**
   - Built a **Logistic Regression classifier** using scikit-learn.
   - Compared predictions at default threshold (0.5) vs tuned threshold (0.7).

3. **Evaluation**
   - Metrics used:
     - Accuracy
     - Precision
     - Recall
     - F1-score
   - Visualization with **Confusion Matrix**.

---

## 📊 Results
- **Accuracy:** ~78%  
- **Class 0 (Non-diabetic):**
  - Recall = 0.92 (very strong performance)
- **Class 1 (Diabetic):**
  - Recall = 0.48 (weaker performance, some cases missed)
- **Threshold Tuning (0.7):**
  - Increased precision for Class 1  
  - Lowered recall for Class 1  
  - Demonstrated trade-off between false positives and false negatives  

---

## 🔮 Future Improvements
- Handle class imbalance using **SMOTE** or **class weighting**.  
- Experiment with **tree-based models** (Random Forest, XGBoost, LightGBM).  
- Perform **hyperparameter tuning** and **cross-validation** for better performance.  

---
