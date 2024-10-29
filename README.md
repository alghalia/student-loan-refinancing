# Student Loan Repayment Prediction System

This project uses machine learning, specifically neural networks, to predict whether a student loan applicant is likely to repay their refinanced loan. By accurately predicting repayment likelihood, the model can help the company determine more suitable interest rates, lowering financial risk and aligning loan offers with applicants' profiles.

Project Overview

The goal of this project is to build a predictive model that:
- Predicts Loan Repayment Success: Uses various features about applicants to predict their ability to repay loans.
- Assists with Interest Rate Adjustment: By estimating repayment likelihood, the model supports customized interest rate decisions.

Dataset and Features

The dataset, provided in a CSV file, contains information on previous student loan applicants, such as:
- Credit Ranking: The target variable, indicating applicants' credit quality.
- Student Profile Features: Includes academic and personal data that could influence repayment likelihood.

Key Project Steps
This project is divided into four main parts:

1. Data Preparation: Prepare data for neural network modeling by cleaning, splitting, and scaling it.
2. Model Compilation and Evaluation: Design, compile, and evaluate a neural network to predict repayment likelihood.
3. Prediction: Use the trained model to predict loan repayment success.
4. Discussion on Recommendation Systems: Explore ideas for a recommendation system for student loans, discussing potential data and filtering techniques.

Requirements

The project requires the following dependencies:
- Python 3.x
- TensorFlow and Keras for neural network building and evaluation
- scikit-learn for data preprocessing and scaling
- pandas and numpy for data handling and manipulation

Recommended Platform
It is recommended to use Google Colab for this project, as it provides a suitable environment with pre-installed libraries and optional GPU access.

Getting Started

Installation (Local Environment)

If you choose to run the project locally, follow these steps:

1. Clone the repository:
   git clone https://github.com/yourusername/neural-network-challenge-1.git

2. Navigate to the project directory:
   cd neural-network-challenge-1

3. Install dependencies:
   pip install -r requirements.txt

Usage Instructions

1. Upload the Dataset to Colab: Start by uploading `student_loans_with_deep_learning.ipynb` and the dataset to Google Colab.
2. Data Preparation: Use the notebook to preprocess the data by splitting, scaling, and preparing it for model training.
3. Model Training: Follow the instructions in Part 2 to build and compile a neural network, then train the model using binary cross-entropy loss and Adam optimizer.
4. Model Evaluation: Evaluate the model on test data to determine loss and accuracy.
5. Prediction: Save and reload the model to make predictions on new data, generating a classification report.
6. Discussion: Complete the recommendation system discussion by answering questions on data needs, filtering method, and challenges.

Example Commands

Run the following command to evaluate the model:
   python evaluate_model.py

Make predictions using the saved model:
   python predict.py --input student_data.csv

Project Structure

- data/: Contains sample datasets and any data preparation scripts.
- models/: Stores trained model files (e.g., student_loans.keras).
- scripts/: Python scripts for training, evaluating, and generating predictions.
- student_loans_with_deep_learning.ipynb: Main notebook for building and testing the model.

Part Breakdown

Part 1: Prepare Data
- Load the CSV file and preprocess it using Pandas and StandardScaler for scaling.
- Define feature and target variables.
- Split the data into training and test sets.

Part 2: Compile and Evaluate Model
- Design a neural network using TensorFlow's Keras with two hidden layers.
- Compile the model with binary_crossentropy as the loss function and the Adam optimizer.
- Train the model and evaluate it on test data to measure loss and accuracy.
- Save the trained model to student_loans.keras.

Part 3: Predict Loan Repayment Success
- Reload the saved model and make predictions on the test data.
- Save predictions in a DataFrame, rounding results to binary values (0 or 1).
- Generate a classification report to summarize prediction accuracy.

