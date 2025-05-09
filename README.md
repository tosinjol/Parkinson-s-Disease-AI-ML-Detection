# Machine Learning for Early Diagnosis and Monitoring of Parkinson’s Disease

**Tosin Jolaogun, Florida Agricultural & Mechanical University**

## Abstract
Parkinson’s Disease (PD) is a neurodegenerative disorder affecting motor function due to the loss of dopamine-producing neurons. This study explores machine learning models to predict PD using acoustic voice features and clinical metrics. The models, including Support Vector Machine (SVM), k-Nearest Neighbors (kNN), XGBoost, and Logistic Regression, were tested on datasets containing vocal biomarkers and UPDRS scores. SVM achieved 92% accuracy, highlighting the potential for non-invasive, data-driven approaches for early PD detection.

In further analysis, disease progression was modeled using symptom severity scores (motor_UPDRS), with Gradient Boosting Regressor (GBR) and Support Vector Regressor (SVR) showing strong predictive performance. The results support the role of machine learning in both diagnosing and tracking PD progression.

## Introduction
PD is characterized by motor symptoms such as tremors and rigidity due to dopamine loss. Early diagnosis is difficult as symptoms overlap with other conditions. Diagnostic tools like the Unified Parkinson’s Disease Rating Scale (UPDRS) provide a structured framework for symptom severity assessment. However, non-invasive and accessible tools, including voice analysis, offer potential improvements. This study investigates machine learning’s role in PD detection and monitoring.

## Data and Preprocessing
This study uses two datasets:
- **“parkinsons.data”**: Acoustic voice features from 195 recordings of 31 individuals.
- **“parkinsons_updrs.data”**: Includes clinical symptom progression data and acoustic features.

Data preprocessing involved scaling features, removing non-numerical columns, and reducing multicollinearity to optimize model performance.

## Methodology
Various models, including SVM, kNN, XGBoost, and Logistic Regression, were applied to the **“parkinsons.data”** dataset to predict PD. The models were evaluated based on accuracy, precision, recall, and F1-score. Among the models tested, SVM performed best, with an accuracy of 92%.

For regression tasks, the **“parkinsons_updrs.data”** dataset was used to model disease progression. GBR and SVR models were employed to predict motor_UPDRS scores, with the GBR model showing strong performance (R² = 0.75 for motor_UPDRS).

## Results
- **Classification**: SVM achieved 92% accuracy, followed by kNN (89%), with XGBoost and Logistic Regression at 82%.
- **Regression**: The GBR model significantly improved performance using cross-validation, achieving an MSE of 16.32 for motor_UPDRS and 25.08 for total_UPDRS, with R² scores of 0.75 and 0.78, respectively.

## Conclusion
Machine learning models effectively distinguish between healthy individuals and PD patients, with SVM excelling in classification. The regression models showed potential for monitoring PD progression. These findings demonstrate machine learning’s capability to enhance early diagnosis and symptom tracking, offering promising applications for clinical use in PD and potentially other diseases.

## Full Paper
For more detailed findings, [read the full paper here](link-to-full-paper).
