# Predicting-Power-Plant-Energy-Output-Using-Machine-Learning
Predicting Power Plant Energy Output Using Machine Learning AI Product Manager Certification — Capstone Modeling Project

## Project Overview

Combined Cycle Power Plants use gas and steam turbines to generate electricity. Operational efficiency depends on accurately forecasting power output based on changing environmental conditions.

In this project, I develop and evaluate machine learning models that predict net hourly electrical energy output (in megawatts) using ambient sensor data. This supports more efficient production planning and better alignment between energy supply and expected demand.

🎯 Business Objective

Enable power plant operators to:

Improve forecasting accuracy

Reduce wasted fuel and operational costs

Optimize workforce and maintenance scheduling

Support data-driven environmental and energy planning

Better predictions → more reliable, cost-efficient power delivery.

🧠 Machine Learning Approach

This is a supervised regression task. Input features:

Feature	Description
AT	Temperature (°C)
V	Exhaust Vacuum (cm Hg)
AP	Ambient Pressure (mbar)
RH	Relative Humidity (%)
Target output:
PE — Net hourly energy output (MW)

Methodology
Step	Description
Data Inspection	Confirmed clean and complete dataset (9,568 rows)
Feature/Target Split: All four environmental variables used as inputs
Train/Test Split	80% training / 20% test
Baseline Model	Linear Regression
Final Model	Random Forest Regressor (improved performance)
Evaluation Metric	RMSE — Root Mean Squared Error

Model Performance
Model	RMSE (MW)	Improvement
Linear Regression	4.503	Baseline
Random Forest	3.231	✅ ~29% increase in prediction accuracy

Key Insights

Temperature (AT) and Exhaust Vacuum (V) are the largest drivers of output variability

The plant’s efficiency decreases as temperature and vacuum increase

Tree-based models more effectively capture nonlinear energy-production behavior
