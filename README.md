# 🫀 Framingham Heart Disease Prediction

[![Python 3.8+](https://img.shields.io/badge/Python-3.8%2B-blue.svg)](https://www.python.org/)
[![Scikit-Learn](https://img.shields.io/badge/Library-Scikit--Learn-orange.svg)](https://scikit-learn.org/)
[![Pandas](https://img.shields.io/badge/Library-Pandas-red.svg)](https://pandas.pydata.org/)

## 📌 Project Overview
This project implements a **Logistic Regression** model to predict the 10-year risk of Coronary Heart Disease (CHD). The analysis is based on the **Framingham Heart Disease Dataset**, which includes clinical measurements and lifestyle factors of over 3,700 residents from Framingham, Massachusetts.

## 📊 Dataset Features
The model utilizes the following clinical and demographic features:
* **Sex_male**: Patient gender (1 = Male, 0 = Female).
* **Age**: Age of the patient in years.
* **CigsPerDay**: Average number of cigarettes smoked per day.
* **TotChol**: Total serum cholesterol levels.
* **SysBP**: Systolic blood pressure.
* **Glucose**: Blood glucose levels.
* **TenYearCHD (Target)**: Binary indicator (1 = High Risk, 0 = Low Risk).

## 🛠️ Data Preprocessing & Modeling
According to the notebook implementation:
1. **Cleaning**: The `education` column was removed, and rows with missing values (NaN) were dropped to ensure data quality.
2. **Standardization**: Features were scaled using `StandardScaler` to ensure the Logistic Regression model treats all clinical units equally.
3. **Training**: The data was split into **70% training** and **30% testing** sets.
4. **Classification**: A Logistic Regression model was trained to predict the probability of heart disease.

## 📈 Performance Results
The model achieved the following metrics on the test set:
* **Model Accuracy**: ~84.9%.
* **Confusion Matrix**:
    * **True Negatives**: 943 (Successfully identified low-risk patients).
    * **True Positives**: 14 (Identified high-risk patients).
    * **Note**: The high accuracy is largely driven by the majority class (No CHD), while the recall for the positive class remains low (~8%).



## 🚀 How to Use
1. **Data Requirements**: Place the `framingham.csv` file in the same directory as the notebook.
2. **Install Dependencies**:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
3.Run: `Open Heart disease prediction.ipynb` in any Jupyter environment or Google Colab and run all cells.
