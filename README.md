# My-eCornell-Portfolio
Includes my Jupyter Notebook assignments from Machine Learning Foundations

In the DefineAndSolveMLProblem I used the [bookReviewsData.csv](https://github.com/user-attachments/files/21499136/bookReviewsData.csv) dataset to create a NLP model!

📊 Census Income Classification
This project explores a real-world binary classification task using the 1994 U.S. Census Income dataset. The goal is to predict whether an individual's income exceeds $50K per year based on demographic and employment-related features. The project follows the full machine learning lifecycle from data exploration to model evaluation.

📁 Dataset
File: censusData.csv

Source: UCI Machine Learning Repository (modified version used in curriculum)

🎯 Problem Definition
Type: Supervised Learning

Task: Binary Classification

Target Variable: income_binary

0 → income ≤ $50K

1 → income > $50K

🔑 Features
Continuous:
age, fnlwgt, education-num, capital-gain, capital-loss, hours-per-week

Categorical (one-hot encoded):
workclass, education, marital-status, occupation, relationship, race, sex_selfID, native-country

⚙️ ML Workflow
🧼 Data Preprocessing
Missing numerical values imputed with column means

Dropped rows with incomplete categorical data

Target variable encoded using LabelEncoder

One-hot encoded categorical features

Standardized features using StandardScaler

🔍 Feature Selection
Used a Random Forest classifier to rank and select the top 50 most important features

🤖 Models Implemented
1. Neural Network (TensorFlow/Keras)
3 hidden layers with ReLU activation

Included Batch Normalization and Dropout

Trained for 115 epochs

Optimizers tested: SGD and Adam

Performance:

Test Accuracy: ~83.9%

Training and validation curves closely aligned

2. Logistic Regression (Baseline)
Implemented using sklearn.linear_model.LogisticRegression

Simple, fast, and interpretable

Performance:

Test Accuracy: ~84.2%

📊 Evaluation
Primary Metric: Accuracy

Visualizations:

Training vs. validation loss and accuracy

Predicted probabilities vs. actual labels

✅ Key Takeaways
Model simplicity: Logistic Regression performed just as well as the more complex neural network

Preprocessing impact: Proper feature scaling and encoding were crucial

Fairness implications: Predicting income based on demographics invites ethical considerations and potential bias

🛠️ Tech Stack
Python 3

Pandas, NumPy

Scikit-learn

TensorFlow / Keras

Matplotlib, Seaborn

📚 Notes
This project was completed as part of Lab 8 in a Machine Learning course. The lab involved defining a predictive problem, preparing a full ML pipeline, and analyzing both model performance and fairness concerns.
