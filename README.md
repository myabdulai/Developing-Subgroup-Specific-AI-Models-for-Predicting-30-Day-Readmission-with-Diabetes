<h2><strong>📖 Overview</strong></h2>

This project develops global and subgroup-specific machine learning models to predict 30-day hospital readmission among diabetic patients using the UCI Diabetes 130-US Hospitals dataset. Hospital readmission is a critical quality metric, and early identification of high-risk patients can significantly improve care coordination and reduce healthcare costs.

By stratifying patients according to their primary diagnosis including Circulatory, Respiratory, and Endocrine/Nutritional/Metabolic/Immune (ENMI) categories—the project demonstrates that subgroup-specific models provide superior predictive accuracy, stronger recall, and more clinically interpretable feature importance patterns compared to a single global model. These results highlight the value of personalized, diagnosis-specific AI models in clinical decision support.

<h2><strong>🎯 Project Objectives</strong></h2>

Develop subgroup-specific AI models for predicting 30-day hospital readmission.
Stratify patients based on primary diagnostic categories: Circulatory, Respiratory, and ENMI.
Compare subgroup model performance vs. global model performance using standardized machine-learning evaluation metrics.
Identify distinct risk factors relevant to each subgroup to support targeted interventions.
Enhance clinical decision support by generating more accurate and personalized predictions.

<h2><strong>🧹 Data Preparation & Preprocessing</strong></h2>

Cleaned and preprocessed all dataset variables.
Removed features with excessive missingness (e.g., weight, medical specialty).
Encoded and regrouped categorical variables to reduce sparsity and improve model performance.
Converted medication features into meaningful binary indicators.
Prevented data leakage by retaining only the first encounter per patient, ensuring independence between observations.

<h2><strong>🤖 Model Development</strong></h2>

<strong>Algorithms Implemented</strong>

Logistic Regression

Linear SVM

KNN

Decision Tree

Random Forest

XGBoost

LightGBM

<strong>Models Built</strong>

Global model (entire dataset)

Circulatory subgroup model

Respiratory subgroup model

ENMI subgroup model

<strong>Modeling Techniques</strong>

SMOTE to mitigate class imbalance

5-fold cross-validation for robust internal evaluation

Confidence intervals for all performance metrics

<h2><strong>📈 Evaluation & Interpretation</strong></h2>

<strong>Metrics Used</strong>

Accuracy

Precision

Recall

F1-score

ROC-AUC

<strong>Outputs Generated</strong>

ROC curves

Feature importance visualizations

Confusion matrices

Classification reports

<h2><strong>🛠️ Technologies Used</strong></h2>

Python (NumPy, Pandas, Scikit-learn)
Ensemble Models: Random Forest, XGBoost, LightGBM
Balancing Technique: SMOTE
Visualization: Matplotlib, Seaborn
Development Environment: Jupyter Notebook

<h2><strong>⚡ Challenges Faced</strong></h2>

Managing class imbalance in readmission outcomes
Avoiding patient-level data leakage from repeated encounters
Working with high-cardinality clinical variables
Maintaining performance consistency across all diagnostic subgroups
Interpreting subgroup-specific clinical patterns and model behavior

<h2><strong>📊 Cross-Validation Performance Summary</strong></h2>

Across all machine-learning algorithms tested, Random Forest consistently emerged as the strongest and most reliable model for both global and subgroup analyses. While LightGBM and XGBoost achieved perfect precision and competitive AUC values, their lower recall and F1-scores made Random Forest the superior model overall. Logistic Regression and Linear SVM showed substantially weaker discrimination, whereas KNN and Decision Tree models produced moderate but less stable results.

Below is the summary of best-performing Random Forest models across all groups:

⭐ <strong>Global Model – Best Overall Global Performance</strong>
Accuracy: 0.924
Precision: 0.978
Recall: 0.869
F1-score: 0.920
ROC-AUC: 0.964

⭐ <strong>Circulatory Model – Best Circulatory Performance</strong>
Accuracy: 0.933
Precision: 0.981
Recall: 0.884
F1-score: 0.930
ROC-AUC: 0.968

⭐ <strong>Respiratory Model – Highest Performance Across All Groups</strong>
Accuracy: 0.959
Precision: 0.992
Recall: 0.925
F1-score: 0.957
ROC-AUC: 0.987

⭐ <strong>ENMI Model – Strong, Balanced Subgroup Performance</strong>
Accuracy: 0.945
Precision: 0.976
Recall: 0.912
F1-score: 0.943
ROC-AUC: 0.982

<h3><strong>🧠 Insights from Cross-Validation</strong></h3>

Random Forest consistently dominated performance across all models.
The Respiratory subgroup achieved the highest metrics overall, suggesting a particularly strong signal in this diagnostic group.
The ENMI subgroup also demonstrated excellent recall and AUC, indicating robust discriminative ability.
The Global model performed well but was outperformed by subgroup models in nearly every metric.
Non-ensemble models showed limited generalization power across clinical subgroups.

<h2><strong>📊 Trained Models Performance on Untouched 20% Test Dataset</strong></h2>

The final trained models were evaluated on a completely unseen 20% test dataset. While subgroup models showed clear advantages during cross-validation, their performance converged on the test set, demonstrating similar generalization patterns across all diagnostic groups.

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

## 👥 Contributors
- Mohammed Yushawu Abdulai  
- Peter Mvuma
