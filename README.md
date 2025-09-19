# Customer Churn Analysis & Prediction
## 🚀 Introduction

Customer churn is a critical challenge for businesses in today’s competitive environment. This project demonstrates how data engineering, analytics, and machine learning can be combined to:
- Understand customer behavior
- Identify churn drivers
- Predict customers likely to churn
- Provide actionable insights via Power BI dashboards

The workflow covers the entire pipeline — ETL in SQL Server → Data Exploration → Power BI Visualization → Machine Learning (Random Forest) → Predicted Data Visualization.

## 🗂️ Project Workflow
Step 1 – ETL Process (SQL Server)

Load raw CSV data into SQL Server using Import Wizard.

Create stg_Churn staging table and clean data (handling nulls, encoding values).

Load clean data into prod_Churn table.

Create SQL Views (vw_ChurnData, vw_JoinData) for Power BI & ML integration.

Step 2 – Power BI Transformation

Create calculated columns (Churn Status, Monthly Charge Range).

Create mapping tables for Age Groups, Tenure Groups, and Services.

Unpivot service columns for analysis.

Step 3 – Power BI Measures

Total Customers

New Joiners

Total Churn

Churn Rate

Step 4 – Power BI Dashboards

Executive Summary Dashboard:

KPIs (Customers, Joiners, Churn, Churn Rate)

Demographic (Gender, Age Group)

Account Info (Payment Method, Contract, Tenure Group)

Geographic (Top 5 States by churn rate)

Churn Distribution (Category, Reason)

Services usage & churn impact

Churn Reason Tooltip Page

Step 5 – Machine Learning (Python, Jupyter Notebook)

Model: Random Forest Classifier

Libraries: pandas, numpy, matplotlib, seaborn, scikit-learn, joblib

Preprocessing: Label Encoding, Train/Test Split

Evaluation: Confusion Matrix, Classification Report, Feature Importance

Predictions on new joiner dataset (vw_JoinData)

Step 6 – Predicted Data Visualization (Power BI)

Import predictions back into SQL/CSV

Dashboard includes demographic, account info, and geographic breakdown of predicted churners

🎯 Project Goals

Build a complete ETL pipeline in SQL Server

Create insightful Power BI dashboards for churn analysis

Develop a Random Forest ML model to predict churners

Enable businesses to design targeted retention strategies

📌 Key Metrics

Total Customers

Total Churn & Churn Rate

New Joiners

Predicted Churners

👥 Target Audience

This project focuses on a telecom dataset, but the techniques are industry-agnostic. Retail, finance, healthcare, and subscription-based businesses can adapt the methodology to improve customer retention & loyalty.

🎨 Design Colors
#4A44F2  
#9B9FF2  
#F2F2F2  
#A0D1FF  

⚙️ Tools & Technologies

SQL Server & SSMS (ETL, Data Cleaning, Views)

Power BI (Visualization, Insights, Dashboarding)

Python (scikit-learn, pandas, seaborn) (Machine Learning)

GitHub (Version Control, Documentation)

📸 Sample Dashboards

👉 (Add screenshots of your Power BI dashboards here)

📂 Repository Structure
📁 data/                 # Raw & cleaned datasets  
📁 sql/                  # SQL scripts (ETL, transformations, views)  
📁 notebooks/            # Jupyter notebooks for ML model  
📁 dashboards/           # Power BI files (.pbix) & images  
📄 README.md             # Project documentation  

🔮 Future Enhancements

Test additional ML models (XGBoost, LightGBM, Neural Networks)

Automate ETL with SQL Agent Jobs / Airflow

Deploy ML model as an API service

Enable real-time churn prediction with Power BI + ML pipeline integration

🙌 Acknowledgements

Microsoft SQL Server & SSMS

Microsoft Power BI

Python & Open-Source Libraries

Inspiration from real-world telecom churn datasets
