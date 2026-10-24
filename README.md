# Telco Customer Churn Prediction: Random Forest Classifier

**Student Name:** Rhydham Shukla  
**Course:** Machine Learning August 2026 Batch Program  
**Institution:** Unlox Academy  
**Dataset:** Kaggle Telco Customer Churn Dataset (7,043 rows, 21 columns)  

## Project Overview
This project delivers an end to end machine learning classification pipeline predicting customer churn for a telecommunications firm. All file paths use clean relative paths, allowing the executed notebook to run in any environment without machine-specific directory dependencies.

Following mentor feedback on the previous submission, this update introduces:
1. Decision threshold optimization tuning the cutoff from 0.50 to 0.55, increasing precision from 51.5% to 54.5% (exceeding the 0.52 benchmark) while retaining peak F1 score (0.634) and eliminating 48 false alarm calls.
2. Fully executed Jupyter Notebook (`Telco_Customer_Churn_Random_Forest.ipynb`) containing all outputs and embedded visualizations.
3. A concise, one page summary report (`Rhydham_Shukla_Minor_Project_4_Report.pdf`) free of boilerplate or disclaimers.

## Key Performance Results
* **5-Fold Stratified Cross-Validation ROC-AUC:** 0.8439
* **Test Set ROC-AUC:** 0.8439
* **Standard Cutoff (0.50):** Accuracy 74.7%, Precision 51.5%, Recall 80.5%, F1 0.628, False Positives 284
* **Optimized Cutoff (0.55):** Accuracy 76.8%, Precision 54.5%, Recall 75.7%, F1 0.634 (Peak), False Positives 236

## Top Predictive Features
1. `Contract_Two year`: Lowest churn propensity (2.8%)
2. `tenure`: Longer tenure drastically reduces churn probability
3. `TotalCharges`: Reflects overall customer relationship value
4. `MonthlyCharges`: Higher monthly costs drive higher cancellation rates
5. `Contract_One year`: Moderate churn rate (11.3%)

## Repository Structure
* `Telco_Customer_Churn_Random_Forest.ipynb`: Executed Jupyter Notebook with all outputs and figures.
* `WA_Fn-UseC_-Telco-Customer-Churn.csv`: Kaggle Telco dataset.
* `Rhydham_Shukla_Random_Forest_Model.joblib`: Serialized trained model with metadata.
* `Rhydham_Shukla_Minor_Project_4_Report.pdf`: 1-page executive summary PDF report.
* `requirements.txt`: Environment package dependencies.

## Installation & Execution
```bash
pip install -r requirements.txt
jupyter notebook Telco_Customer_Churn_Random_Forest.ipynb
```
