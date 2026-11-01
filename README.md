# diabetes-prediction-logistic-regression
Machine Learning project for diabetes outcome classification using Logistic Regression, Python, Pandas and Scikit-learn.
# 🩺 Diabetes Prediction Using Logistic Regression

A Machine Learning classification project that predicts diabetes outcomes using the **Pima Indians Diabetes Dataset** from Kaggle. This project demonstrates data preprocessing, feature scaling, Logistic Regression, and model evaluation using Python.

## 📌 Project Overview

The objective of this project is to build a Logistic Regression model that predicts whether a person belongs to the diabetes-positive or diabetes-negative class based on various health-related numerical features.

- **0:** No Diabetes
- **1:** Diabetes

## 🎯 Objectives

- Understand and explore a real-world dataset.
- Perform data cleaning and preprocessing.
- Handle invalid zero values using median imputation.
- Apply feature scaling using StandardScaler.
- Train a Logistic Regression classification model.
- Evaluate model performance using classification metrics.
- Interpret model coefficients.

## 📂 Dataset Information

**Dataset:** Pima Indians Diabetes Database  
**Source:** Kaggle

- Total records: 768
- Input features: 8
- Target variable: Outcome

### Features Used

| Feature | Description |
|---|---|
| Pregnancies | Number of pregnancies |
| Glucose | Glucose concentration |
| BloodPressure | Diastolic blood pressure |
| SkinThickness | Skin fold thickness |
| Insulin | Insulin level |
| BMI | Body Mass Index |
| DiabetesPedigreeFunction | Diabetes pedigree function |
| Age | Age of the individual |

**Target:** Outcome

## 🛠️ Technologies Used

- Python
- Google Colab
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

## ⚙️ Project Workflow

1. **Data Loading:** Imported the Kaggle dataset using Pandas.
2. **Exploratory Data Analysis:** Inspected dataset structure, statistics, and missing values.
3. **Data Cleaning:** Identified invalid zero values in measurement columns and replaced them with missing values.
4. **Missing Value Handling:** Applied median imputation.
5. **Feature and Target Separation:** Separated input features (X) and target variable (y).
6. **Train-Test Split:** Divided the dataset into 80% training and 20% testing data.
7. **Feature Scaling:** Applied StandardScaler.
8. **Model Training:** Trained Logistic Regression with class balancing.
9. **Prediction:** Generated predictions using the test dataset.
10. **Evaluation:** Evaluated the model using classification metrics, confusion matrix, and ROC-AUC.
11. **Coefficient Analysis:** Examined the influence of individual features on model predictions.

## 📊 Model Performance

The Logistic Regression model achieved the following results on the test dataset:

| Evaluation Metric | Score |
|---|---:|
| Accuracy | 73.38% |
| Precision | 60.32% |
| Recall | 70.37% |
| F1-Score | 64.96% |
| ROC-AUC | 0.813 |

### Confusion Matrix

|  | Predicted 0 | Predicted 1 |
|---|---:|---:|
| Actual 0 | 75 | 25 |
| Actual 1 | 16 | 38 |

### Feature Coefficient Analysis

The coefficient analysis showed that:

- **Glucose (+1.183):** Highest positive coefficient.
- **BMI (+0.710):** Second-highest positive coefficient.
- Pregnancies (+0.373) also showed a positive coefficient.

These coefficients describe relationships learned by the model; they do not establish causation.

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Working with real-world datasets.
- Data cleaning and handling missing values.
- Understanding feature scaling.
- Implementing Logistic Regression.
- Evaluating classification models.
- Understanding precision, recall, F1-score, and ROC-AUC.
- Interpreting model coefficients.

## ⚠️ Limitations

This project uses a relatively small historical dataset representing a specific population. The model is developed strictly for educational purposes and machine learning practice.

**This model is not intended for medical diagnosis or clinical decision-making.**

## 🚀 How to Run the Project

1. Clone this repository:

   ```bash
   git clone YOUR_GITHUB_REPOSITORY_URL
   ```

2. Open the project notebook (`.ipynb`) in Google Colab or Jupyter Notebook.

3. Install the required libraries if they are not already available:

   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn
   ```

4. Download the Pima Indians Diabetes Dataset from Kaggle.

5. Upload `diabetes.csv` to your Colab environment.

6. Execute the notebook cells sequentially to reproduce the workflow and results.

## 👨‍💻 Author

**B. Abhishek**

B.Tech – Computer Science and Engineering  
Learning Artificial Intelligence and Machine Learning

---

⭐ *This project is part of my ongoing journey of learning Python, Machine Learning, and practical AI development.*
