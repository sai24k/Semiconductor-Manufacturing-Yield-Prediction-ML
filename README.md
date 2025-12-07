# 🏭 Capstone Project 2 – Semiconductor Manufacturing Yield Prediction  

## 📌 Project Description  
This project focuses on **predicting pass/fail yield outcomes** in a semiconductor manufacturing process using high-dimensional sensor data.  
The dataset contains readings from **591 different sensors/features** per production entity. Not all signals are equally important, so the project also aims to perform **feature selection** to identify the most relevant signals impacting yield.  

The ultimate goal is to:
- Build accurate machine learning models for yield prediction.
- Reduce dimensionality for efficiency.
- Provide insights for process improvement to increase throughput, reduce production costs, and enhance quality control.  

---

## 📂 Dataset  

**File:** `signal-data.csv`  
- **Shape:** 1567 rows × 592 columns  
- **Features:** 591 continuous sensor readings  
- **Target:** Pass/Fail outcome  
  - `-1` → Pass  
  - `1` → Fail  

---



## 🛠 Procedure 

1. **Data Understanding & Cleaning**  
   - Loaded `sensor-data.csv` and inspected shape, types, and missing values.  
   - Removed irrelevant columns based on domain knowledge.  
   - Filled missing values using median imputation.  

2. **Exploratory Data Analysis (EDA)**  
   - Checked class balance and visualized target distribution.  
   - Performed univariate, bivariate, and multivariate analysis using plots and statistical summaries.  

3. **Data Preprocessing**  
   - Split predictors (X) and target (y).  
   - Applied **SMOTE** to balance classes.  
   - Standardized features using StandardScaler.  
   - Performed train-test split and validated data consistency.  

4. **Model Training & Optimization**  
   - Trained multiple models (**Random Forest, SVM, Naïve Bayes**).  
   - Used **cross-validation** for performance estimation.  
   - Applied **GridSearchCV** for hyperparameter tuning.  

5. **Model Evaluation**  
   - Compared models on accuracy, precision, recall, and F1-score.  
   - Selected **Random Forest** as the final model.  
   - Saved the model using `joblib` for future use.  

---



## 🛠 Tech Stack & Libraries  
- **Python 3.x**  
- NumPy  
- Pandas  
- Matplotlib & Seaborn  
- Scikit-learn  
- Imbalanced-learn (SMOTE)  
- Joblib / Pickle  



## 📷 Sample Output Images 

### **1. Classification report – Best Model**  
![Confusion Matrix](output-images/classification-report.png)  

### **2. Model Comparison Training vs Testing Accuracy**  
![Model Comparison](output-images/training-and-testing-accuracy.png)  

### **3. Class 0 – Precision Comparison**  
![Class 0 Precision](output-images/class0-precision.png)  

### Class 0 – Recall Comparison**  
![Class 0 Recall](output-images/class0-recall.png)  

### Class 0 – F1 Score Comparison**  
![Class 0 F1 Score](output-images/class0-f1.png)  

---

### **4. Class 1 – Precision Comparison**  
![Class 1 Precision](output-images/class1-precision.png)  

###  Class 1 – Recall Comparison**  
![Class 1 Recall](output-images/class1-recall.png)  

### Class 1 – F1 Score Comparison**  
![Class 1 F1 Score](output-images/class1-f1.png)  



---

## 📊 Project Presentation

**PowerPoint Presentation:** [Download Presentation](https://github.com/sai24k/Semiconductor-Manufacturing-Yield-Prediction-ML/releases)

- Comprehensive overview of the project methodology
- Visual representations of key findings
- Model performance summary and recommendations

---

## 📄 Project Report

**Detailed Project Report:** [View on Google Drive](https://drive.google.com/)

- Complete analysis and methodology documentation
- Comprehensive results and findings
- Recommendations for future improvements

---
