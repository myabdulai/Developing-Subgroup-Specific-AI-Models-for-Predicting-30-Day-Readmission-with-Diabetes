📌 README.md (Ready to Upload)
Developing Subgroup-Specific AI Models for Predicting 30-Day Readmission in Patients with Diabetes

This project focuses on building machine-learning models—both global and subgroup-specific—to predict 30-day hospital readmission among diabetic patients. Using the UCI Diabetes 130-US Hospitals dataset, the work investigates whether specialized AI models based on primary diagnostic subgroups (Circulatory, Respiratory, ENMI) outperform a traditional global model. The project is part of the SAT 5141 Clinical Decision Modeling coursework.

📂 Project Overview

Hospital readmissions within 30 days are a major quality and cost concern in diabetes care. Traditional global predictive models often fail to capture heterogeneity across patients with different underlying conditions.
This project proposes subgroup-specific AI modeling to improve precision, interpretability, and clinical relevance.

The project includes:

Comprehensive data preprocessing and feature engineering

Global model and three subgroup-specific models

Multiple machine-learning algorithms (Logistic Regression, Decision Tree, SVM, KNN, Random Forest, XGBoost, LightGBM)

Cross-validation performance comparison

ROC-AUC curves, feature importance plots, and test-set evaluation

Interpretation of clinical implications

🧠 Key Objectives

Develop and compare global vs. subgroup-specific ML models

Circulatory

Respiratory

Endocrine/Nutritional/Metabolic/Immunity (ENMI)

Evaluate model performance using:

Accuracy

Precision

Recall

F1-score

ROC-AUC

Confidence intervals on all metrics

Identify the most predictive clinical features for each subgroup.

Assess whether subgroup modeling improves predictive capability compared to pooled modeling.

📊 Dataset

Source: UCI Machine Learning Repository – Diabetes 130-US Hospitals dataset

Records: 101,766 encounters from 71,518 adult patients

Time span: 1999–2008

Features: 47 clinical, demographic, diagnostic, lab, and utilization variables

Outcome: 30-day readmission (binary: <30 days vs. >30/NO)

Data preparation steps included:

Removing high-missingness variables

Encoding categorical variables

Regrouping low-frequency categories

Handling missing values via imputation

Converting medications to binary

Keeping only each patient’s first encounter to prevent label leakage


Project Proposal Report 1- Grou…

🛠 Models Used

Each subgroup and the global dataset were trained using:

Logistic Regression

Linear SVM

KNN

Decision Tree

Random Forest

XGBoost

LightGBM

Techniques applied:

SMOTE for balancing classes

5-fold cross-validation

Train/test split (80/20)

Confidence intervals for performance metrics

Feature importance analysis

🏆 Summary of Key Findings

Random Forest consistently outperformed all other methods across global and subgroup models.

The Respiratory subgroup model showed the highest overall performance:

Accuracy: 0.959 ± 0.005

Recall: 0.925 ± 0.007

F1-score: 0.957 ± 0.005

ROC-AUC: 0.987 ± 0.002


Project Proposal Report 1- Grou…

Subgroup-specific models outperformed the global model in cross-validation, revealing stronger discriminatory power when focusing on specific diagnoses.

On the unseen 20% test set, models performed similarly, showing accuracy around 0.90–0.91, with ENMI achieving slightly higher recall and F1.


Project Proposal Report 1- Grou…

📈 Included Visualizations

ROC curves with 95% confidence intervals

Feature importance graphs for each subgroup

Confusion matrices

Classification reports
