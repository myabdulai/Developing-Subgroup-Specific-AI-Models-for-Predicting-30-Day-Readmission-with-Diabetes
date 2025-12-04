📖 Overview

This project develops global and subgroup-specific machine learning models to predict 30-day hospital readmission among diabetic patients using the UCI Diabetes 130-US Hospitals dataset.

Current clinical prediction models often treat all diabetic patients as a homogeneous group, which can mask important differences across diagnostic categories. This project demonstrates that subgroup-specific AI models provide improved accuracy, recall, F1-scores, and ROC-AUC performance across key patient groups—including Circulatory, Respiratory, and Endocrine/Metabolic/Immune (ENMI) subpopulations.

The system aims to:

🔍 Identify high-risk diabetic patients more accurately

📊 Improve clinical decision support for early intervention

🧠 Reveal subgroup-level risk patterns through feature importance

🏥 Provide evidence for personalized and data-driven disease management

🎯 Project Objectives
1. Data Preparation & Preprocessing

Clean and preprocess the Diabetes 130-US Hospitals dataset

Remove high-missingness variables (e.g., weight, medical specialty)

Encode categorical features and regroup low-frequency categories

Convert medication variables to meaningful binary indicators

Reduce label leakage by using only the first encounter per patient 

Project Proposal Report 1- Grou…

2. Model Development

Implement multiple ML models:

Logistic Regression

SVM (Linear)

KNN

Decision Tree

Random Forest

XGBoost

LightGBM

Build global and three subgroup-specific models:

Circulatory

Respiratory

ENMI (Endocrine/Nutritional/Metabolic/Immune)

Apply SMOTE, 5-fold cross-validation, and confidence interval estimation

3. Evaluation & Interpretation

Assess model performance using:

Accuracy

Precision

Recall

F1-score

ROC-AUC

Generate:

📈 ROC curves (with 95% confidence intervals)

🧩 Feature importance plots

🟦 Confusion matrices

📝 Classification reports

🛠️ Technologies Used

Programming: Python (Pandas, NumPy, Scikit-learn)

Ensemble Models: Random Forest, XGBoost, LightGBM

Visualization: Matplotlib, Seaborn

Data Balancing: SMOTE (imblearn)

Notebook Environment: Jupyter Notebook

⚡ Challenges Faced

Handling large categorical medical variables with many low-frequency groups

Preventing data leakage caused by repeated patient encounters

Managing severe class imbalance in the 30-day readmission outcome

Ensuring stability of cross-validated model performance across subgroups

Interpreting diagnostic-specific risk factors from high-dimensional datasets

✅ Outcomes Achieved
1. Subgroup Models Outperformed the Global Model

The Respiratory subgroup model showed the highest performance:

Accuracy: 0.959 ± 0.005

Recall: 0.925 ± 0.007

F1-score: 0.957 ± 0.005

ROC-AUC: 0.987 ± 0.002


Project Proposal Report 1- Grou…

2. Random Forest Emerged as the Best Overall Model

Across all subgroups, Random Forest:

Achieved the highest accuracy, recall, and F1­-score

Provided the most stable cross-validation performance

Demonstrated superior ROC-AUC values

3. Successful Model Interpretation & Clinical Insights

Feature importance revealed key predictors such as:

Number of inpatient visits

Time in hospital

Glucose serum levels

Insulin and metformin usage

Subgroups revealed unique risk profiles, supporting personalized clinical strategies

4. Test Set Validation Showed Consistent Performance

All optimized models maintained 0.90–0.91 accuracy on unseen data.
