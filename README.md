# 🫀 Heart Disease Prediction Using Machine Learning

This project aims to predict the presence of heart disease in patients using the **UCI Heart Disease dataset**. The dataset contains demographic information and clinical measurements of patients. The project involves data analysis, preprocessing, and applying various machine learning algorithms to make predictions. Important factors affecting heart disease are also analyzed.

---

## Project Objectives

- Load and inspect the dataset
- Check for missing or erroneous data
- Perform Exploratory Data Analysis (EDA) and visualize the data
- Identify the target variable
- Transform categorical variables appropriately
- Scale numerical features
- Build and train machine learning models
- Compare model performances
- Select and interpret the best-performing model
- Analyze key factors affecting heart disease

---

## Dataset Features

| Column | Description |
|--------|-------------|
| id | Unique identifier for each patient |
| age | Age of the patient |
| origin | Data collection center |
| sex | Gender (Male / Female) |
| cp | Chest pain type (typical angina, atypical angina, non-anginal, asymptomatic) |
| trestbps | Resting blood pressure (mm Hg) |
| chol | Serum cholesterol (mg/dl) |
| fbs | Fasting blood sugar > 120 mg/dl (True / False) |
| restecg | Resting ECG result (normal, ST-T abnormality, left ventricular hypertrophy) |
| thalach | Maximum heart rate achieved |
| exang | Exercise-induced angina (True / False) |
| oldpeak | ST depression induced by exercise |
| slope | Slope of the peak exercise ST segment |
| ca | Number of major vessels colored by fluoroscopy (0–3) |
| thal | Thalassemia status (normal, fixed defect, reversible defect) |
| num | Target variable (0: No heart disease, 1: Heart disease) |

**Goal:** Develop a reliable machine learning model to aid early detection of heart disease using clinical data, contributing to healthcare decision support systems.

---

## Best Performing Model: Random Forest

| Model | Accuracy | Precision | Recall | F1-score |
|-------|---------|-----------|--------|----------|
| RandomForest | 0.853 | 0.844 | 0.902 | 0.872 |
| GaussianNB | 0.842 | 0.861 | 0.853 | 0.857 |
| AdaBoost | 0.826 | 0.837 | 0.853 | 0.845 |
| GradientBoosting | 0.815 | 0.804 | 0.882 | 0.841 |
| LogisticRegression | 0.815 | 0.804 | 0.882 | 0.841 |
| KNN | 0.734 | 0.757 | 0.765 | 0.761 |
| DecisionTree | 0.728 | 0.755 | 0.755 | 0.755 |

---

## Results and Model Performance

Machine learning models including Logistic Regression, Decision Tree, K-Nearest Neighbors, AdaBoost, Gradient Boosting, Gaussian Naive Bayes, and Random Forest were trained and evaluated using accuracy, precision, recall, and F1-score. Among them, **Random Forest achieved the best balance** with ~85% accuracy and 0.87 F1-score.

Additionally, a **deep learning approach** using an Artificial Neural Network (ANN) was implemented for tabular clinical data. The ANN consists of fully connected dense layers with **ReLU activation** in hidden layers and **sigmoid activation** in the output layer for binary classification. The model was trained using **binary cross-entropy loss** and the **Adam optimizer**.

---

## Deep Learning Model Architecture

- **Feedforward neural network** with multiple hidden layers
- Hidden layers use **ReLU activation** for non-linear learning
- Output layer uses **sigmoid activation** for probability output
- **Binary cross-entropy loss** and **Adam optimizer**

**Training Results:**

- Training accuracy reached ~99% across epochs
- Validation accuracy fluctuated between 70–75%
- Test accuracy achieved **96.84%**, demonstrating strong general performance
- Slight validation fluctuations are attributed to the small dataset size and limited validation examples

---

## Conclusion

- Random Forest is the most balanced machine learning model (~85% accuracy, F1-score 0.87)
- ANN deep learning model achieved 96.8% accuracy and successfully captured complex non-linear relationships
- The project demonstrates the potential of both machine learning and deep learning to predict heart disease and support clinical decision-making
