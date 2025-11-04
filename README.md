🌍 AI-Based Energy Consumption Predictor

📘 Overview

This project develops an AI-driven system to predict next-day household energy consumption using the UCI Individual Household Electric Power Consumption Dataset. It leverages Random Forest and XGBoost regressors, integrates contextual factors such as temperature, humidity, holidays, and weekends, and provides explainable insights through SHAP.

Beyond forecasting, the system estimates daily electricity costs using a time-based tariff model and evaluates CO₂ emissions, promoting both cost savings and environmental sustainability.

⚡ Features
📊 Next-Day Energy Prediction using ML models (Random Forest, XGBoost)
🌤️ Contextual Awareness — weather, weekends, holidays included
🧠 Explainable AI (SHAP) — interprets feature importance transparently
💰 Cost Optimization — tariff-based daily cost and cheapest hour detection
🌿 Sustainability Module — CO₂ emission estimation and reduction potential
📈 Visual Analytics — energy trends, SHAP plots, and cost variation charts
💾 Model Persistence — saves trained models with joblib for future use

🧩 Tech Stack
Language: Python 3
Libraries: pandas, numpy, scikit-learn, xgboost, shap, seaborn, matplotlib, joblib, holidays
Dataset: UCI Household Electric Power Consumption

⚙️ Workflow
Data Acquisition: Download and extract UCI dataset
Preprocessing: Merge date-time, clean missing values, aggregate to daily data
Feature Engineering: Add lag, rolling mean, weather, and calendar features
Model Training: Train Random Forest & XGBoost regressors
Evaluation: Compute MAE and RMSE for both models
Explainability: Apply SHAP for global and local feature interpretation
Optimization: Estimate daily cost & identify cheapest usage hours
Sustainability: Estimate CO₂ emissions and savings potential
Model Saving: Export trained models (.pkl files)

📂 Outputs
rf_next_day.pkl — Trained Random Forest Model
xgb_next_day.pkl — Trained XGBoost Model
scaler_next_day.pkl — Standard Scaler
shap_feature_importance.csv — Feature importance summary
Visual plots for trends, costs, and SHAP explanations
