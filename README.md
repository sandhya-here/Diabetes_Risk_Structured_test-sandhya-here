# Predicting Risk of Heart Disease using the Framingham Dataset

## 📌 Objective

The goal of this project is to build a machine learning model to predict the **10-year risk of coronary heart disease (CHD)** using the Framingham Heart Study dataset. This predictive model helps identify individuals at risk based on key health indicators.

## 🧠 Dataset Overview

The dataset contains anonymized medical data for individuals, including:

* Demographics (e.g., age, sex)
* Health indicators (e.g., BMI, blood pressure, cholesterol)
* Behavioral factors (e.g., smoking, diabetes)

**Target Variable**:

* `TenYearCHD`: Binary label indicating whether the patient developed CHD within 10 years.

**Sample Columns**:

```
male, age, education, currentSmoker, cigsPerDay, BPMeds, prevalentStroke,
prevalentHyp, diabetes, totChol, sysBP, diaBP, BMI, heartRate, glucose, TenYearCHD
```

## ⚙️ Workflow

1. **Data Cleaning**:

   * Removed rows with missing values.
   * Dropped any unnecessary columns (e.g., IDs if present).

2. **Encoding**:

   * Used one-hot encoding for categorical features (e.g., `education`).

3. **Feature Scaling**:

   * Applied `StandardScaler` to normalize the feature values.

4. **Model Training**:

   * Trained a **Logistic Regression** classifier to predict heart disease risk.

5. **Evaluation**:

   * Used metrics like **Accuracy**, **Confusion Matrix**, and **Classification Report**.

## 📊 Results

* **Accuracy**: \~75%
* **Recall for Class 1 (At risk)**: High — good for medical predictions
* **Precision for Class 0**: Low — model struggles to identify non-risk cases
* The model has a bias toward predicting patients as at risk.

## ✅ Dependencies

```
pandas
numpy
scikit-learn
matplotlib (optional)
seaborn (optional)
```

---

## ✍️ Author

Sandhya Burje
