# Loan Approval Predictor

This project predicts whether a loan application will be approved or rejected using a **Logistic Regression** machine learning model. It is designed to provide quick predictions based on user-provided inputs, simulating a simplified version of a credit scoring system used by banks and financial institutions.

## How it Works

1. **Data Processing**  
   The model is trained on historical loan data, which includes features such as:
   - `person_age`: Applicant's age
   - `person_gender`: Applicant's gender
   - `person_education`: Highest education level
   - `person_income`: Annual income
   - `person_home_ownership`: Type of home ownership (OWN, RENT, MORTGAGE, OTHER)
   - `loan_amnt`: Requested loan amount
   - `loan_intent`: Purpose of the loan (EDUCATION, HOMEIMPROVEMENT, MEDICAL, PERSONAL, VENTURE)
   - `credit_score`: Applicant's credit score  

   Categorical features are encoded using **Label Encoding** or **One-Hot Encoding**, while numerical features are scaled using **StandardScaler** to normalize the data.

2. **Model Training**  
   - The model uses **Logistic Regression** with class balancing to handle imbalanced loan approval outcomes.
   - The dataset is split into training and testing sets to evaluate model performance.
   - Key evaluation metrics such as **F1 Score**, **Accuracy**, and **Confusion Matrix** are calculated to ensure reliability.

3. **User Input Prediction**  
   - Users enter their details through prompts.  
   - Input values are encoded and scaled in the same way as the training data.  
   - The trained model predicts whether the loan will be **Approved ✅** or **Rejected ❌** in real-time.

## Features

- Handles both **numerical** and **categorical** inputs.  
- Provides **real-time loan approval prediction**.  
- Includes **model evaluation metrics** for transparency.  
- Easy to extend for additional features or deployment as a web app.

This project demonstrates the complete workflow from **data preprocessing**, **model training**, to **real-time prediction** based on user input.
