# Loan-Default-Prediction
A machine learning project to predict loan defaults using logistic regression, PCA, and feature engineering
# Loan Default Prediction Project

## Project Overview
In this project, we aim to predict whether a borrower will default on a loan. By analyzing various features of the borrower and loan details, we build a machine learning model to help financial institutions make smarter lending decisions.

## Dataset Information
The project uses two main files:

- **train.csv**: This file contains the training data, which includes features like borrower details and loan information, as well as the target variable, 'Default'. This tells us whether the borrower defaulted on the loan.
- **test.csv**: This file contains the test data. It’s similar to the training data but doesn't include the target variable 'Default'. We use this data to evaluate the model’s performance.

## Approach

### Feature Engineering
- **Handling Missing Values**: The dataset might have some missing values, and we’ve filled those gaps with appropriate strategies (like replacing missing numerical values with the mean).
- **One-Hot Encoding**: We’ve converted categorical features into numerical format using one-hot encoding, so that they can be used by the machine learning model.

### Model Selection
- **Logistic Regression**: For this binary classification problem, we used logistic regression, which is great at predicting probabilities, like whether someone will default on a loan.

### Evaluation Metrics
- **ROC AUC Score**: To measure the model’s performance, we used the ROC AUC score. It helps us understand how well the model distinguishes between the two classes (default vs. no default). A score closer to 1 means better performance.

## Results
Our model achieved an ROC AUC score of 0.75 on the validation set, which is a solid result. It means the model is doing a good job at predicting loan defaults. It performed well when tested with the unseen test data too.

## How to Run the Project

### Setting Up
1. First, clone the repository to your local machine:
    ```bash
    git clone https://github.com/nehahh/loan-default-prediction.git
    ```

2. Next, install the necessary libraries by running:
    ```bash
    pip install -r requirements.txt
    ```

3. Finally, run the project by executing:
    ```bash
    python main.py
    ```

This will start the script, which loads the dataset, processes it, trains the model, and evaluates its performance.

## Files in This Repository

- **main.py**: This is the core Python script where all the magic happens. It handles loading the data, cleaning it, training the model, and evaluating it.
- **requirements.txt**: This file contains a list of all the Python libraries you’ll need to run the project (like pandas, scikit-learn, numpy, and others).
- **train.csv**: The dataset used to train the model.
- **test.csv**: The dataset used to test and evaluate the model’s predictions.
- **README.md**: This file, which gives you all the details about the project and how to run it.
