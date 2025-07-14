# Loan-Risk-Analysis
J.P. Morgan Quantitative Research Virtual Experience (Forage)
Loan Risk Analysis - J.P. Morgan Job Simulation (Forage)

This repository contains my solutions and insights from the J.P. Morgan Data for Good Job Simulation on the Forage platform. The goal was to evaluate and model financial risk associated with loan defaults using real-world inspired datasets.

🚀 Overview

The simulation was divided into two technical tasks:

🧠 Task 3: Predicting Probability of Default & Expected Loss
Model: Logistic Regression
Objective: Predict the likelihood that a loan will default
Metrics Used:
PD (Probability of Default)
EAD (Exposure at Default)
LGD (Loss Given Default)
Output: Calculate Expected Loss = PD × LGD × EAD for a sample loan

🔍 Task 4: Risk Segmentation via FICO Scores
Method: Dynamic Programming & Log-Likelihood Estimation
Objective: Identify optimal FICO score segments that separate high- and low-risk borrowers
Steps:
Aggregate defaults by score
Apply cumulative counting
Use dynamic programming to maximize total log-likelihood over 10 segments
Extract segmentation breakpoints (FICO thresholds)

🛠 Tech Stack
Python
NumPy & Pandas
Scikit-learn (Logistic Regression, train_test_split, roc_auc_score)
Math (log-likelihood functions)

📊 Example Outputs
Task 3: Expected Loss Output
{
  'PD (Probability of Default)': 0.3542,
  'Expected Loss ($)': 1593.90
}

Task 4: FICO Score Segment Thresholds
[850, 842, 830, 810, 785, 758, 730, 700, 660, 610, 550]

📁 Files
task3_logistic_model.py – Code to train logistic regression and compute expected loss
task4_segment_fico.py – Dynamic programming for segmentation
Loan_Data.csv – Sample dataset (replace with path)
README.md – This file

📌 Key Learnings
Risk modeling in real-world finance involves more than prediction: interpretability and threshold analysis are key.
Dynamic programming can help optimize decision boundaries in classification problems.
Combining ML and statistical methods leads to deeper insights.

📎 Credits
This project is based on the J.P. Morgan Data for Good Simulation hosted on Forage.

💼 Author
Samarth Melsingare 
