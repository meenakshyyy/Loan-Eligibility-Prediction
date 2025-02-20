# Loan Eligibility Prediction Model

## Project Overview
The **Loan Eligibility Prediction Model** is designed to automate the loan approval process for **Dream Housing Finance Company**. By analyzing customer details provided in the application form—such as **income, credit history, loan amount, and other demographic factors**—this model predicts whether a loan should be approved. The goal is to help the company efficiently identify eligible customers and streamline the loan approval process.

---

## Dataset
The dataset was provided as part of a **hackathon conducted by Analytics Vidhya**.

### Dataset Description
The dataset consists of customer details, including **income, credit history, education, and loan information**. The **train dataset** contains labeled loan approval outcomes (`Loan_Status`), while the **test dataset** consists of unlabeled customer data for which predictions are to be made.

### Key Features
- **Applicant Information:** Gender, Marital Status, Education, Number of Dependents, Employment Status
- **Financial Details:** Applicant Income, Co-applicant Income, Loan Amount, Loan Term
- **Credit & Property Information:** Credit History, Property Area (Urban, Semi-Urban, Rural)
- **Target Variable:** `Loan_Status` (Y/N) – Whether the loan is approved

---

## Technologies Used
This project is implemented in **Python** using the following libraries:

- **Jupyter Notebook** – For data exploration and model development
- **Pandas** – Data manipulation and preprocessing
- **Matplotlib & Seaborn** – Data visualization
- **Scikit-Learn (sklearn)** – Machine learning algorithms and evaluation metrics

---

## Installation & Setup Guide

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/meenakshyyy/Loan-Eligibility-Prediction.git
cd loan-prediction-model
```

### 2️⃣ Install Dependencies
Ensure you have **Python 3.x** installed, then install all required libraries:
```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

### 3️⃣ Running the Jupyter Notebook
To explore the dataset and train models, launch Jupyter Notebook:
```bash
jupyter notebook
```
Open the file (`Loan-prediction-model.ipynb`) and execute the cells sequentially.

---

## Model Performance & Results
The model was evaluated with and without outlier removal.

### Without Outlier Removal:
- **Logistic Regression**:77.8% accuracy
- **Naïve Bayes**:75.69% accuracy
- **Random Forest (RF)**:76.38% accuracy
- **K-Nearest Neighbors (KNN)**:70.83% accuracy

### With Outlier Removal
- **Logistic Regression**:72.22% accuracy
- **Naïve Bayes**:68.75% accuracy
- **Random Forest (RF)**:70.1% accuracy
- **K-Nearest Neighbors (KNN)**:66.67% accuracy

Further improvements can be made through **hyperparameter tuning, feature engineering, and deep learning approaches**.

---

## Conclusion
This project successfully predicts loan eligibility based on customer information. The model provides an automated way to assist financial institutions in assessing loan applications efficiently. Future enhancements may include **more advanced feature engineering, handling imbalanced data, and deploying the model as a real-time API**.
