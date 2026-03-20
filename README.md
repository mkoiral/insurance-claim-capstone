# Insurance Claim Prediction Using Machine Learning

### Risk Modeling and Cost Prediction with Structured Healthcare Data

---

## Project Overview

Insurance companies must accurately predict claim likelihood and expected costs to manage financial risk and optimize pricing strategies. This project applies machine learning techniques to predict whether a policyholder is likely to file a claim and to estimate insurance charges using demographic and health-related data.

Multiple machine learning models were developed and compared to identify the most effective approach for structured tabular data.

---

## Problem Statement

Traditional insurance risk assessment relies on manual rules and limited statistical models, which may fail to capture complex relationships between customer attributes and claim behavior.

The goal of this project is to predict insurance claim likelihood, estimate expected costs, identify key drivers of risk, and compare model performance across multiple machine learning approaches.

---

## Dataset

The dataset contains approximately 1,300 records with features including:

- Age  
- Sex  
- BMI  
- Number of children  
- Smoking status  
- Region  

Targets include:

- `insuranceclaim` for classification  
- `charges` for regression  

---

## Preprocessing and Feature Engineering

Key preprocessing steps include:

- Handling missing values without dropping data  
- One-hot encoding of categorical variables  
- Feature engineering based on exploratory data analysis  
- Standardization of numerical features  
- Train-test split (80/20) for model evaluation  

All preprocessing steps were applied consistently across training and testing datasets.

---

## Models Evaluated

- Logistic Regression (baseline model)  
- Decision Tree (nonlinear model)  
- Random Forest (final model)  

---

## Model Performance

### Classification (Claim Prediction)

| Model | Accuracy | Precision | Recall | F1 Score |
|------|--------|----------|--------|---------|
| Logistic Regression | ~0.88 | ~0.90 | ~0.89 | ~0.90 |
| Decision Tree | ~0.99 | ~0.99 | ~0.99 | ~0.99 |
| Random Forest | ~0.96 | ~0.95 | ~0.97 | ~0.96 |

### Regression (Cost Prediction)

| Model | RMSE | R² |
|------|------|----|
| Linear Regression | ~5958 | ~0.81 |
| Decision Tree | ~6345 | ~0.78 |
| Random Forest | ~4253 | ~0.90 |

---

## Key Findings

Smoking status is the most influential feature affecting both insurance charges and claim likelihood. Individuals who smoke have significantly higher costs compared to non-smokers.

BMI shows a strong positive relationship with insurance charges, particularly at higher levels. This indicates that increased BMI is associated with higher medical risk and cost.

Age is positively correlated with insurance charges, suggesting that older individuals tend to incur higher healthcare expenses.

Random Forest models effectively capture nonlinear relationships and interactions between features, leading to improved performance compared to simpler models.

---

## Why This Matters

This project demonstrates how machine learning can enhance decision-making in the insurance industry by improving risk assessment, optimizing pricing strategies, and enabling better customer segmentation.

---

## Limitations

- Relatively small dataset  
- Limited feature set (no medical history)  
- Potential bias in demographic variables  

---

## Future Work

- Incorporate additional features such as medical history and claims history  
- Apply SHAP for model interpretability  
- Explore advanced models such as XGBoost  
- Deploy the model for real-time prediction  

---

## Project Structure

-insurance_claim_capstone_one_data_wrangling.ipynb
-insurance_EDA_continuation_FINAL_v2.ipynb
-insurance_feature_engineering_from_eda.ipynb
-insurance_modeling.ipynb
-metrics.csv
-Insurance_Claim_Capstone_Final_Report.pdf
-insurance_claim_capstone_presentation.pptx
-README.md

