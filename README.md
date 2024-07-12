# Telecom Customer Churn Predictor

This project implements a Deep Learning model using TensorFlow and Keras to predict customer churn in a Telecom industry context. Customer Churn prediction is crucial for businesses to retain customers and optimize resources effectively.

## DataSet
The dataset provides comprehensive customer information from a Telecom company, focusing on various aspects that influence Churn behavior:
- **Demographic Information**: Includes customer demographics such as age, gender, and marital status.
- **Services Subscribed**: Details on the telecom services subscribed by customers, such as internet service type (DSL, Fiber Optic), streaming services, online security, and backup services.
- **Contract and Billing**: Information about contract terms (month-to-month, yearly), billing methods (paperless billing), and payment methods.
- **Churn Label**: The dataset includes a binary `Churn` column indicating whether a customer has churned or not.

The dataset is instrumental for developing predictive models because it captures diverse customer attributes that influence churn decisions. This information allows for deep insights into customer behavior and facilitates proactive churn management strategies.

## Motivation
The telecom industry faces challenges in customer retention due to high churn rates, impacting revenue and operational efficiency. Predictive models like the one developed in this project enable telecom companies to identify customers at risk of churn early. This proactive approach empowers businesses to implement targeted retention strategies and enhance customer satisfaction.

## Project Overview

1. **Data Preprocessing and EDA**: 
    - Handled missing values and transformed categorical variables.
    - Performed extensive EDA to understand the distribution and relationships within the data.
    - Visualized categorical and numerical features with respect to the target variable 'Churn'.

2. **Feature Engineering**:
    - Encoded categorical variables using Label Encoding and One-Hot Encoding.
    - Applied ordinal encoding for specific features with an inherent order.
    - Log-transformed skewed numerical features for better model performance.

3. **Model Building**:
    - Constructed a sequential neural network model using Keras.
    - Utilized Keras Tuner for hyperparameter tuning to identify the optimal model architecture.
    - Implemented early stopping to prevent overfitting and ensure the best model is selected.

4. **Hyperparameter Tuning**:
    - Used Keras Tuner to explore various configurations of the neural network.
    - *Install Keras Tuner using `pip install keras-tuner`*
    - Evaluated the model based on validation accuracy and selected the best model with the optimal hyperparameters.
    - This process helped in refining the model to achieve better performance.

5. **Model Evaluation**:
    - Evaluated the model using various metrics such as accuracy, AUC, and confusion matrix.
    - Plotted the training and validation accuracy to visualize the model's performance over epochs.
    - Generated and displayed the confusion matrix and ROC curve for a comprehensive evaluation.

## Evaluation Metrics and Plots

- **Classification Report**: Provides precision, recall, F1-score, and support for each class.
- **Confusion Matrix**: Visual representation of true positives, true negatives, false positives, and false negatives.
- **ROC Curve**: Illustrates the model's performance across different thresholds.

## Conclusion
This project exemplifies the application of Deep Learning in predicting Telecom Customer Churn, highlighting the significance of data-driven approaches in mitigating customer attrition. By leveraging advanced techniques and rigorous evaluation, it contributes to enhancing retention strategies and operational efficiency in the telecom industry.
