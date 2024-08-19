
# Credit Card Fraud Detection Pipeline

## Overview

This project demonstrates a machine-learning pipeline for detecting fraudulent credit card transactions. The goal is to preprocess the data, build a model, and evaluate its performance in identifying fraudulent transactions.

## Table of Contents

- [Project Structure](#project-structure)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Pipeline](#model-pipeline)
- [Results](#results)

## Project Structure

The repository is structured as follows:
```

├── creditcard.csv # Dataset used for the project
├── CreditCardFraudDetection.ipynb # Jupyter notebook with the pipeline
├── README.md # Project README file

````

## Dataset

The dataset used in this project is the [Credit Card Fraud Detection dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud) from Kaggle. It contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions.

- **Features**: V1, V2, … V28 are the principal components obtained with PCA.
- **Target**: The target variable is `Class`, where 1 indicates a fraudulent transaction, and 0 indicates a normal transaction.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:

    ```
    git clone https://github.com/yourusername/CreditCardFraudDetection.git
    cd CreditCardFraudDetection
    ```

2. Install the required Python packages:

    ```
    pip install -r requirements.txt
    ```

    Make sure you have Python 3.6+ installed.

## Usage

Open the Jupyter notebook:

```
jupyter notebook notebooks/CreditCardFraudDetection.ipynb
````

Run the notebook cells sequentially to execute the entire pipeline. The notebook includes data preprocessing, exploratory data analysis, model building, evaluation, and results visualization.

## Model Pipeline

1. **Data Exploration**: Load and explore the dataset to understand its structure.
2. **Data Preprocessing**: Handle missing values, drop duplicates, and handle class imbalance.
3. **Feature Engineering**: Apply transformations to make the data more suitable for modeling.
4. **Model Building**: Build and train a classification model using XGBoost.
5. **Model Evaluation**: Evaluate the model using a confusion matrix and classification report.

## Results

The model's performance is measured using accuracy, precision, recall, and F1-score. The results are visualized using a confusion matrix and other relevant plots. These metrics help in understanding how well the model can detect fraudulent transactions.
