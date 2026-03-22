# heart-disease-project-
"Heart disease prediction using machine learning and EDA (Exploratory Data Analysis)"

# Heart Disease Analysis (EDA, Data Cleaning & Preprocessing)

Exploratory Data Analysis on Heart Disease Dataset

---

## 📌 Project Overview
This project focuses on analyzing a heart disease dataset using Exploratory Data Analysis (EDA) techniques.  
The main goal is to understand the data, identify issues, clean it, and prepare it for machine learning models.

---

## 📊 Dataset Information
- Total records: 918  
- Total features: 12  

### Features:
- Age – Age of patient  
- Sex – Gender  
- ChestPainType – Type of chest pain  
- RestingBP – Resting blood pressure  
- Cholesterol – Cholesterol level  
- FastingBS – Fasting blood sugar  
- RestingECG – ECG results  
- MaxHR – Maximum heart rate  
- ExerciseAngina – Exercise-induced angina  
- Oldpeak – ST depression  
- ST_Slope – Slope of ST segment  
- HeartDisease – Target (0 = No, 1 = Yes)

---

## ⚙️ Work Performed

### 🔹 1. Data Loading
- Loaded dataset using pandas  
- Viewed first rows using `.head()`  

---

### 🔹 2. Data Understanding
- Checked column names using `.columns`  
- Checked dataset shape → (918, 12)  
- Used `.info()` to understand data types  
- Found mix of numerical and categorical data  

---

### 🔹 3. Data Quality Check
- Checked missing values → No null values  
- Checked duplicate values → No duplicates  

---

### 🔹 4. Data Visualization
- Bar plot of HeartDisease (class distribution)  
- Histograms of:
  - Age  
  - RestingBP  
  - Cholesterol  
  - MaxHR  
- Correlation heatmap to see relationships between features  

---

### 🔹 5. Data Issues Found
- Some values were incorrect:
  - Cholesterol = 0 (not possible in real life)  
  - RestingBP = 0 (not possible)  

---

### 🔹 6. Data Cleaning
- Replaced invalid values (0) with mean values  
- Rounded values for better readability  

---

### 🔹 7. Feature Engineering
- Converted categorical variables into numerical form  
- Prepared dataset for model training  

---

### 🔹 8. Feature Scaling
- Applied StandardScaler on:
  - Age  
  - RestingBP  
  - Cholesterol  
  - MaxHR  
  - Oldpeak  
- This helps improve model performance  

---

## 📈 Key Insights
- Dataset has no missing or duplicate values  
- Some features had incorrect zero values → fixed  
- Heart disease cases are slightly imbalanced  
- Features like Oldpeak and MaxHR show relation with heart disease  

---

## 🛠️ Tools & Libraries
- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Seaborn  
- Scikit-learn  

---

## 📁 Project Files
- heart.csv → dataset  
- heart_disease_analysis.ipynb → main notebook  
- README.md → project description  

---

## 🚀 Future Work
- Apply classification models (Logistic Regression, Random Forest)  
- Evaluate accuracy  
- Deploy model using web app  
