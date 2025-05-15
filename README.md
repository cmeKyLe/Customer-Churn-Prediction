# Customer Churn Prediction & Insights Dashboard

## Overview
This project analyzes a real‑world telecom dataset to understand why customers leave and to predict which ones are at risk of churn. Through data cleaning, visual exploration, and machine learning, it produces a reusable model and a ready‑to‑use dataset for business reporting.

---

## What I Did

1. **Data Preparation**  
   - Cleaned raw customer records (fixed billing fields, handled missing values, preserved customer IDs)  
   - Exported a polished dataset for modeling  

2. **Exploratory Analysis**  
   - Charted churn rates by tenure, billing, contract type, and service options  
   - Highlighted key patterns (e.g. month‑to‑month contracts and lack of support services drive churn)  

3. **Model Building**  
   - Trained and compared several algorithms to predict churn risk  
   - Tuned the top performer to balance correctly identifying churners with minimizing false alarms  

4. **Deployment Artifacts**  
   - Saved a processing pipeline + model (`churn_pipeline.pkl`)  
   - Generated a final predictions file (`dashboard_data.csv`) with churn probabilities and flags  

---

## Project Structure

dataset/
├── WA_Fn-UseC_-Telco-Customer-Churn.csv # Original raw data
├── cleaned_telco_churn.csv # Cleaned data for modeling
└── dashboard_data.csv # Final churn scores & binary flags

models/
└── churn_pipeline.pkl # Serialized data pipeline + model

notebooks/
├── 01_EDA.ipynb # Data cleaning & exploratory analysis
├── 02_Modeling.ipynb # Model training & evaluation
└── test.ipynb # Sanity checks & validation



---

## How to Get Started

1. **Clone the repo** to your machine  
2. **Open** the notebooks in order:
   - `01_EDA.ipynb` — clean and explore the data  
   - `02_Modeling.ipynb` — build and evaluate models  
   - `test.ipynb` — validate final outputs  
3. **Inspect** the outputs in `dataset/` and `models/`

---

## Tools & Technologies

- **Python** (pandas, scikit‑learn, imbalanced‑learn, matplotlib, seaborn)  
- **SQL** for data slicing and preprocessing  
- **Jupyter Notebooks** for analysis and reporting  

---

## Key Findings

- **High risk** among short‑tenure customers and those on month‑to‑month contracts  
- **Billing and support** features (high monthly charges, lack of tech support) strongly influence churn  
- **Optimized model** delivers clear churn risk scores for targeted retention campaigns  

---

## Next Steps

- (Optional) Build an interactive dashboard using the `dashboard_data.csv` output  
- Deploy the saved pipeline behind an API for real‑time scoring  
- Monitor performance and retrain as new data becomes available  

