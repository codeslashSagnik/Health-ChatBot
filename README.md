# Heart Disease Prediction Health Chatbot

## Overview
This project aims to develop a health chatbot that assists users in understanding their risk of heart disease. By integrating machine learning models with chatbot functionalities, users can input their health metrics and receive an instant evaluation of their heart disease risk. The chatbot provides insights based on a dataset that includes various health parameters such as age, cholesterol level, resting blood pressure, and more.

## Detailed Architecture

### 1. Data Collection and Preprocessing:
- **Source:** The dataset, `heart-disease.csv`, contains various health metrics related to heart disease.
- **Features:** age, sex, chest pain type (cp), resting blood pressure (trestbps), cholesterol level (chol), fasting blood sugar (fbs), resting electrocardiographic results (restecg), maximum heart rate achieved (thalach), exercise induced angina (exang), ST depression induced by exercise (oldpeak), slope of the peak exercise ST segment (slope), number of major vessels colored by fluoroscopy (ca), and thalassemia (thal).
- **Target Variable:** `target` - Indicates whether the person has heart disease (1) or not (0).
- **Data Integrity:** Before feeding the data into the model, it was ensured that there were no missing values.

### 2. Exploratory Data Analysis:
Utilized various visualization techniques to understand the distribution and relationships of the features. The dataset's balance, correlation matrix, feature distributions, and feature-target relationships were studied extensively to gain insights into the data.

### 3. Model Development:
Several machine learning models were trained and tested on the dataset:
- Logistic Regression
- K-Nearest Neighbors (KNN)
- Support Vector Classifier (SVC)
- Decision Tree Classifier
- Gaussian Naive Bayes
- Random Forest Classifier
- XGBoost Classifier

Based on the performance metrics, Logistic Regression was chosen as the final model for integration with the chatbot due to its highest accuracy and interpretability.

### 4. Chatbot Integration:
- **User Interface:** Users can interact with the chatbot through a simple and intuitive interface. They can provide their health metrics, and the chatbot will utilize the machine learning model in the backend to predict the risk.
- **Response Generation:** The chatbot processes user input, feeds it to the predictive model, and generates a response indicating the user's risk level.
- **Feedback Mechanism:** Users can provide feedback on the predictions, allowing for continuous model improvement.

### 5. Deployment:
- **Backend Server:** The chatbot and machine learning model are hosted on a server that processes user requests in real-time.
- **Continuous Learning:** The system can be updated with more recent data or improved models to ensure accurate predictions over time.

### 6. Future Enhancements:
- **Feature Engineering:** New features can be introduced or existing ones can be transformed to improve model accuracy.
- **Advanced Models:** Deep learning models or more sophisticated algorithms can be tested for further accuracy improvements.
- **User Feedback Integration:** Incorporate user feedback to retrain and enhance the model's accuracy.

By integrating machine learning with a user-friendly chatbot interface, this project provides valuable health insights directly to the users, assisting them in understanding and potentially mitigating their heart disease risks.
