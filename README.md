##Insurance Claim Prediction Using Machine Learning
##Risk Modeling and Cost Prediction with Structured Healthcare Data
#Project Overview
Insurance companies must accurately predict claim likelihood and expected costs to manage financial risk and optimize pricing strategies. This project applies machine learning techniques to predict whether a policyholder is likely to file a claim and to estimate insurance charges using demographic and health-related data. Multiple machine learning models were compared to identify the most effective approach for structured tabular data.

##Problem Statement
Traditional insurance risk assessment relies on manual rules and limited statistical models, which may fail to capture complex relationships between customer attributes and claim behavior. This project focuses on predicting claim likelihood, estimating insurance charges, identifying key influencing factors, and comparing model performance.

##Dataset
The dataset contains approximately 1,300 records with features including age, sex, BMI, number of children, smoking status, and region. The targets include insuranceclaim for classification and charges for regression.
Preprocessing and Feature Engineering
Data preprocessing included handling missing values, encoding categorical variables, feature engineering based on exploratory data analysis, and standardizing numerical features. The dataset was split into training and testing sets to ensure model evaluation reliability.
Models Evaluated
Logistic Regression was used as a baseline model due to its simplicity and interpretability. Decision Tree models were used to capture nonlinear relationships. Random Forest was selected as the final model due to its robustness, ability to reduce overfitting, and strong performance.

Model Performance
For classification, Logistic Regression achieved moderate performance, Decision Tree showed very high accuracy, and Random Forest provided a strong balance between accuracy and generalization. For regression, Random Forest achieved the lowest error and highest explanatory power compared to other models.
Key Findings
Smoking status is the most influential feature affecting both insurance charges and claim likelihood. Individuals who smoke have significantly higher costs. BMI shows a strong positive relationship with insurance charges, especially at higher levels. Age contributes to increasing costs and risk over time. Random Forest models effectively capture nonlinear relationships and interactions between features, leading to better performance compared to simpler models.
Visualizations
The project includes visualizations such as distribution of insurance charges, comparison of charges by smoking status, relationships between charges and BMI and age, model performance comparisons, confusion matrix, ROC curve, feature importance plots, and regression diagnostics.
Why This Matters
This project demonstrates how machine learning can improve decision-making in insurance by enabling better risk assessment, pricing strategies, and customer segmentation. It highlights the importance of data-driven approaches in modern insurance analytics.
Limitations
The dataset is relatively small and lacks additional features such as medical history. There may also be bias in demographic variables which could influence predictions.
Future Work
Future improvements include incorporating additional data sources, applying advanced interpretability techniques such as SHAP, testing more advanced models, and deploying the model for real-time use.

Project Structure
insurance_claim_capstone_one_data_wrangling.ipynb
insurance_EDA_continuation_FINAL_v2.ipynb
insurance_feature_engineering_from_eda.ipynb
insurance_modeling.ipynb
metrics.csv
Insurance_Claim_Capstone_Final_Report.pdf
insurance_claim_capstone_presentation.pptx
README.md


