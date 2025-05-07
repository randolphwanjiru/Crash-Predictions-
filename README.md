# Crash-Predictions-
🚗 Injury Severity Prediction from Crash Data
This project uses supervised machine learning to classify injury severity from structured crash data. The goal is to predict whether an occupant in a motor vehicle crash will sustain an injury based on crash and vehicle characteristics.

📌 Problem Statement
Motor vehicle crashes result in millions of injuries annually. Accurately predicting injury outcomes can improve emergency response, insurance assessments, and safety planning. However, the data is often imbalanced and noisy, making prediction difficult.

This project formulates the problem as a binary classification task:

1: Injury
0: No Injury
🧠 Key Features Used
Seatbelt usage
Airbag deployment status
Crash type (e.g., frontal impact)
Vehicle weight and year
Occupant demographics

🧪 Methodology
1. Data Preprocessing

Removed missing values
Label encoded categorical variables
Scaled numerical variables with StandardScaler
2. Class Imbalance Handling

Used ADASYN to oversample minority class (No Injury)
4. Models Trained

Logistic Regression (baseline)
Random Forest
XGBoost
LightGBM
Stacked Ensemble (meta-model: Logistic Regression)
5. Threshold Tuning

Tested thresholds: 0.3–0.5
Optimized for recall and precision trade-offs
🧩 Limitations
No Injury class remained difficult to classify with high precision and recall.

✅ Future Work
Integrate SHAP or LIME for feature explainability
Incorporate time, weather, and location features
Test real-time prediction viability in emergency triage contexts
Explore deep learning models or hybrid tabular neural networks
