# Predict the Onset of Diabetes Based on Diagnostic Data

## Project Overview
Diabetes is a chronic health condition affecting millions of people worldwide. In India alone, over 72 million individuals were affected as of 2017, with projections indicating a significant increase in the coming decades. Early diagnosis is essential for effective management and prevention of complications.

This project uses supervised machine learning techniques to predict the onset of diabetes based on diagnostic and physiological data. The aim is to build a reliable classification model that can assist in early detection and healthcare decision-making.

---

## Objective
To develop a machine learning classification model that predicts whether a patient is likely to develop diabetes using medical diagnostic features from the Pima Indians Diabetes Dataset.

---

## Dataset
**Source:** Pima Indians Diabetes Database  
**Type:** Structured medical diagnostic data  

**Target Variable:**  
- `Outcome`  
  - `1` – Diabetic  
  - `0` – Non-Diabetic  

**Features:**  
- Glucose  
- BloodPressure  
- SkinThickness  
- Insulin  
- BMI  
- DiabetesPedigreeFunction  
- Age  

---

## Technologies Used
- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  

---

## Exploratory Data Analysis (EDA)
Exploratory Data Analysis was conducted to understand the dataset and identify patterns and potential issues:
- Examined dataset structure, data types, and summary statistics  
- Identified zero and missing values in medical features  
- Analyzed feature distributions  
- Studied correlations between features and target variable  
- Identified the presence of outliers  

EDA provided insights necessary for effective preprocessing and model building.

---

## Baseline Machine Learning Models
The dataset was split into training and testing sets, and the following baseline classification models were implemented and evaluated using accuracy:

- Logistic Regression  
- K-Nearest Neighbors (KNN)  
- Decision Tree Classifier  
- Random Forest Classifier  

These models served as baseline benchmarks before applying feature engineering techniques.

---

## Feature Engineering
To improve model performance, multiple feature engineering steps were applied:

### Feature Scaling
- MinMaxScaler  
- StandardScaler  

Model performance was evaluated after applying each scaling technique.

### Feature Selection
Based on domain knowledge and relevance to diabetes prediction, the following features were selected:
- Glucose  
- BMI  
- Age  
- Insulin  
- DiabetesPedigreeFunction  

These features are known to have strong medical relevance and predictive power.

### Outlier Removal
- Outliers were detected and removed using the Interquartile Range (IQR) method  
- Models were retrained on the cleaned dataset  
- Performance was re-evaluated after outlier removal  

### Model Improvement Techniques
- Feature scaling  
- Feature selection  
- Outlier handling  
- Ensemble learning using Random Forest  

---

## Results (Current Stage)
- Feature engineering improved model stability and performance  
- Random Forest achieved better accuracy compared to baseline models  
- Data preprocessing played a significant role in improving predictions  

These results represent the current stage of the project and will be further optimized.

---

## Future Work
- Hyperparameter tuning using GridSearchCV  
- Cross-validation  
- Handling class imbalance using SMOTE  
- Feature importance analysis  
- Model deployment  

---

---

## Key Learnings
- End-to-end machine learning workflow implementation  
- Working with real-world medical datasets  
- Importance of data preprocessing and feature engineering  
- Evaluation and comparison of classification models  

---

## Conclusion
This project demonstrates the application of machine learning in the healthcare domain to predict diabetes onset using diagnostic data. With further optimization, such models can contribute to early diagnosis and improved patient care.
