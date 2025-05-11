# Customer Churn Prediction Model

## Project Overview
This project aims to address the challenge of customer churn in the competitive banking landscape by leveraging predictive analytics. Our goal is to develop models that forecast the likelihood of customers leaving the bank and implement targeted retention strategies to safeguard revenue streams and enhance long-term profitability.

## Business Understanding
**Business Problem:** Customer churn poses a significant challenge in the banking industry, leading to loss of revenue generated from lending and financial transactions. Identifying potential churn indicators and implementing preemptive measures is essential to mitigate these risks and maintain a sustainable business model.

**Managerial Decisions:** We propose leveraging predictive analysis techniques to forecast customer churn. By analyzing historical banking data, we aim to develop models that identify high-risk customers early and implement targeted retention strategies, such as personalized engagement, loyalty programs, and tailored incentives.

## Objective
Utilize predictive analytics to forecast customer churn, identify high-risk customers early, and implement targeted retention strategies to safeguard revenue and enhance profitability.

## Dataset
**Source:** Kaggle  
**Description:** The dataset contains 10,000 observations and 12 variables related to customer demographics, account information, and transaction history.

## Methodology
**Data Preprocessing and Analysis:**
- Handled missing values and converted categorical variables to numerical
- Conducted feature selection using correlation analysis

**Model Development:**
- Implemented the Artificial Neural Network
- Deployed using Streamlit

**Results:**
- Enhanced customer retention strategies led to a $1.98 million increase in quarterly revenue
- Demonstrated the effectiveness of machine learning in reducing false positives and accurately identifying at-risk customers

**Recommendations:**
- Personalized retention strategies including targeted incentives
- Referral programs and fee waivers to improve customer loyalty and reduce churn

This project implements an Artificial Neural Network (ANN) to predict customer churn using banking customer data.

## Project Structure
- `experiments.ipynb`: Contains data preprocessing, model training and evaluation
- `prediction.ipynb`: Demonstrates how to make predictions using the trained model
- `app.py`: Streamlit web application for making predictions
- `model.h5`: Saved Keras model
- `*.pkl`: Saved preprocessing objects (encoders, scaler)
- `Churn_Modelling.csv`: Original dataset

## Web Application Usage
To run the Streamlit web application using Command Prompt (cmd):
1. Open Command Prompt
2. Navigate to the project directory
3. Run:
```cmd
streamlit run app.py
```

The application provides an interactive interface to:
- Input customer details
- View churn probability prediction
- Get churn classification (likely/not likely)

## Data Description
The dataset contains customer information including:
- CreditScore
- Geography
- Gender
- Age
- Tenure
- Balance
- NumOfProducts
- HasCrCard
- IsActiveMember
- EstimatedSalary
- Exited (target variable)

## Model Architecture
The ANN model consists of:
1. Input layer (11 features)
2. Hidden layer (64 neurons, ReLU activation)
3. Hidden layer (32 neurons, ReLU activation)
4. Output layer (1 neuron, sigmoid activation)

Trained with:
- Adam optimizer (learning rate=0.01)
- Binary crossentropy loss
- Early stopping callback
- TensorBoard logging

## Results
The model achieves ~86% accuracy on the test set.

## Dependencies
- Python 3.12.7
- TensorFlow 2.18
- scikit-learn
- pandas
- numpy
