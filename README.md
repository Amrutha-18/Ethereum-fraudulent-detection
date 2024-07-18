# Ethereum-fraudulent-detection
Ethereum-fraudulent-detection
│
├── templates
│   ├── index.html
│   ├── result.html
│   └── result_1.html
│
├── Base_code.ipynb
├── app.py
├── model.py
├── amrutha_1.pkl
└── run.py

Overview

This project involves setting up a Flask web application for Ethereum fraud detection. The application allows users to either input data points manually or upload a CSV file to get predictions on whether the transactions are fraudulent or not. The predictions are displayed along with visualizations.

Base code has theimplementation of multiple models and their accuracies.
HTML Templates

index.html: Main page with input form for data points or CSV upload.
result.html: Displays prediction results from CSV file.
result_1.html: Displays prediction results from a single data point.
Flask Application (run.py) : This is the main Python file for the application. It incorporates all necessary functions and configurations.

Key Features:
Imported necessary libraries like Flask, pickle, pandas, and matplotlib.
Configured the Flask application and loaded the pre-trained model.
Defined routes for handling user interactions and predictions.
Implemented logic for predictions and plot generation.

cd path/to/Ethereum-fraudulent-detection
Install Required Packages

Train the Model:
Run the model.py file to generate the pickle file with the trained data model
Run python run.py to access local host
Access the App
Open a browser and go to http://127.0.0.1:5000/ (local host).

Interaction with the Website

Index Page (index.html):
Option to upload a CSV file or enter a single data point.
Form fields for required data.
Submit the form to get predictions and visualizations.

Result Pages:
result.html: Displays output for CSV data.
result_1.html: Displays output for a single data point.

Algorithms Used
Random Forest: Chosen for its robustness, ability to handle complex nonlinear relationships, and high accuracy (96.1%).
SVM: Showcased robust performance with an accuracy of 94.6%.
K-Means: Exhibited limitations with lower accuracy (64.9%).
Naive Bayes: Maintained balanced performance with an accuracy of 86.9%.
KNN: Demonstrated competitive performance with an accuracy of 93.1%.

Random Forest Tuning
Number of Estimators (Trees): Set to 100.
Max Depth of Trees: Adjusted to prevent overfitting.
Minimum Samples per Leaf: Tuned to balance model complexity and generalization.
Training and Testing Set Split: 80% training and 20% testing.
Performance Metrics: Monitored accuracy, recall, precision, error rate, F1 Score, and AUC.
Applicability to Fraud Detection
Feature Importance: Measures significance of each feature.
Nonlinear Relationships: Captures complex patterns of fraud.
Probability Estimation: Provides nuanced understanding of model's predictions.
Ensemble Learning: Reduces overfitting and increases stability.

Main Page:

Upload a CSV file or enter data points manually.
Submit to get predictions and visualizations.

Result Pages:
Displays predictions and pie charts of fraud vs. non-fraud.
By following these steps, you can successfully set up and use the Flask web application for Ethereum fraud detection.
