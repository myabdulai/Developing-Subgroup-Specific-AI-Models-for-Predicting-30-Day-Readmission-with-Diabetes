This project develops global and subgroup-specific machine learning models to predict 30-day hospital readmission among diabetic patients using the UCI Diabetes 130-US Hospitals dataset.

By segmenting patients into diagnostic subgroups (Circulatory, Respiratory, and ENMI), this work demonstrates that subgroup-specific models reveal stronger predictive accuracy, improved recall, and clearer clinical interpretability compared to global modeling alone.

<h2><strong>🎯 Project Objectives</strong></h2>

Develop subgroup-specific AI models for predicting 30-day hospital readmission

Stratify patients by primary diagnosis (circulatory, respiratory, endocrine)

Compare performance of subgroup vs. global models

Identify subgroup-specific risk factors for targeted interventions

Enhance clinical decision support for personalized care


<h2><strong>Data Preparation & Preprocessing</strong></h2>

Cleaned and preprocessed all variables

Removed high-missingness variables

Encoded and regrouped categorical features

Converted medication variables into binary indicators

Prevented data leakage by retaining only each patient's first encounter

<h2><strong>2. Model Development</strong></h2>

Algorithms implemented:

Logistic Regression

Linear SVM

KNN

Decision Tree

Random Forest

XGBoost

LightGBM

Models were built for:

Global dataset

Circulatory subgroup

Respiratory subgroup

ENMI subgroup

Modeling techniques:

SMOTE for class balancing

5-fold cross-validation

Confidence intervals for all metrics

<h2><strong>3. Evaluation & Interpretation</strong></h2>

Metrics used:

Accuracy

Precision

Recall

F1-score

ROC-AUC

Outputs generated:

ROC curves

Feature importance graphs

Confusion matrices

Classification reports

<h2><strong>🛠️ Technologies Used</strong></h2>

Python (NumPy, Pandas, Scikit-learn)

Ensemble Models: Random Forest, XGBoost, LightGBM

Balancing Technique: SMOTE

Visualization: Matplotlib, Seaborn

Development Environment: Jupyter Notebook

<h2><strong>⚡ Challenges Faced</strong></h2>

Addressing class imbalance

Avoiding leakage from repeat patient encounters

Dealing with complex high-cardinality clinical variables

Achieving consistent model performance across subgroups

Interpreting subgroup-specific clinical patterns

<h2><strong>✅ Cross-Validation Results Summary</strong></h2>

The Respiratory subgroup model delivered the best cross-validation performance:

Accuracy: 0.959

Recall: 0.925

F1-score: 0.957

ROC-AUC: 0.987

Random Forest consistently emerged as the strongest algorithm across global and subgroup models, achieving the highest stability and predictive performance.

<h2><strong>📊 Trained Models Performance on Untouched 20% Test Dataset</strong></h2>

The trained models demonstrated consistent performance when evaluated on the unseen 20% test dataset. While subgroup models excelled during cross-validation, their performance converged on the test set, showing similar generalization across all diagnostic groups.

<strong>Global Test Performance:</strong>
Accuracy: 0.90
Precision: 0.55
Recall: 0.51
F1-score: 0.50

<strong>Circulatory Test Performance:</strong>
Accuracy: 0.90
Precision: 0.56
Recall: 0.51
F1-score: 0.50

<strong>Respiratory Test Performance:</strong>
Accuracy: 0.91
Precision: 0.57
Recall: 0.51
F1-score: 0.50

<strong>ENMI Test Performance:</strong>
Accuracy: 0.90
Precision: 0.59
Recall: 0.52
F1-score: 0.52
