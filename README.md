🩺 <strong>Subgroup-Specific AI Models for Predicting 30-Day Readmission in Diabetes Patients</strong>
















<h2><strong>📖 Overview</strong></h2>

This project develops global and subgroup-specific machine-learning models to predict 30-day hospital readmission among diabetic patients using the UCI Diabetes 130-US Hospitals dataset.

It demonstrates that subgroup-specific diagnostic models outperform global models in accuracy, recall, F1-score, and ROC-AUC — offering better clinical interpretability and risk stratification.

<h2><strong>🎯 Project Objectives</strong></h2> <h3><strong>1. Data Preparation & Preprocessing</strong></h3>

Cleaned and preprocessed dataset

Removed high-missingness variables

Encoded and regrouped categorical variables

Converted medications into binary indicators

Prevented label leakage by using only each patient’s first encounter

<h3><strong>2. Model Development</strong></h3>

Models built: Logistic Regression, Linear SVM, KNN, Decision Tree, Random Forest, XGBoost, LightGBM
Subgroup models created for:

Circulatory

Respiratory

ENMI (Endocrine / Nutritional / Metabolic / Immune)

Techniques used:

SMOTE

5-fold cross-validation

Confidence interval estimation

<h3><strong>3. Evaluation & Interpretation</strong></h3>

Performance metrics: Accuracy, Precision, Recall, F1-score, ROC-AUC
Outputs generated:

ROC curves with 95% CI

Feature importance graphs

Confusion matrices

Classification reports

<h2><strong>🛠️ Technologies Used</strong></h2>

Python (NumPy, Pandas, Scikit-learn)

Random Forest, XGBoost, LightGBM

SMOTE for balancing

Matplotlib, Seaborn

Jupyter Notebook

<h2><strong>⚡ Challenges Faced</strong></h2>

Extreme class imbalance

Avoiding leakage from repeated encounters

Highly heterogeneous categorical features

Achieving stable subgroup performance

Interpreting subgroup-specific clinical predictors

<h2><strong>✅ Outcomes Achieved</strong></h2> <h3><strong>1. Subgroup Models Outperformed the Global Model</strong></h3>

The Respiratory subgroup model delivered the best performance:

Accuracy: 0.959

Recall: 0.925

F1-score: 0.957

ROC-AUC: 0.987

<h3><strong>2. Random Forest Was the Best Performing Algorithm</strong></h3>

Achieved consistently highest accuracy, recall, and ROC-AUC across all datasets.

<h3><strong>3. Strong Clinical Interpretability</strong></h3>

Key predictors included:

Number of inpatient visits

Time in hospital

Glucose serum levels

Insulin usage

Number of diagnoses

<h3><strong>4. Consistent Real-World Test Performance</strong></h3>

All final models achieved 0.90–0.91 accuracy on the unseen test set.
