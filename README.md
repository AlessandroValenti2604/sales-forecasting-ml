# sales-forecasting-ml
Machine Learning models for real-world monthly revenue forecasting | Python • Scikit-learn • Power BI



##  Overview
Predictive analytics project developed during my experience as Data Analyst, focused on forecasting monthly revenue to support strategic business decisions. The project combines EDA, machine learning models, and interactive visualizations.

## Business Context
During my role at OpenDoor (Spain) I collaborated with a local company, Cablebox, where I identified the need for accurate revenue forecasting to optimize resource allocation and commercial planning. This project automates the forecasting process and provides actionable insights through an interactive Power BI dashboard.

##  Dataset
- **Source**: Historical sales data from Navision (Intern Software of Cablebox) 
- **Time Period**: 24 months
- **Features**: month, 'Number of Customers, 'Number of transactions', trimester, the month before revenue, the 2 months before revenue, the 3 months before revenue, revenue per client.
- **Target Variable**: Monthly revenue

## 🔧 Technologies & Tools
- **Python 3.9+**
  - Pandas 
  - NumPy
  - Scikit-learn 
  - Matplotlib & Seaborn 
- **Jupyter Notebook** (analysis and experimentation)
- **Power BI** (interactive dashboards)


## Methodology

### 1. Exploratory Data Analysis (EDA)
- Data quality assessment and cleaning
- Temporal patterns identification
- Correlation analysis
- Outlier detection

### 2. Feature Engineering
- Time-based features (month, quarter, seasonality)
- Lag features (previous months revenue)
- Rolling averages (3-month, 6-month)

### 3. Model Development
Implemented and compared multiple algorithms:
- **Linear Regression** (baseline)
- **Random Forest Regressor**
- **XGBRegressor**
- **CatBoostRegressor**
- **LGBMRegressor**

### 4. Model Evaluation
- Metrics: MAE, RMSE, R², MAPE
- Cross-validation (time series split)
- Train/Test split: 80/20

##  Results

### Model Performance
| Model | MAE | RMSE | R² | MAPE |


**Linear Regression**	| 19818.89	143.83	0.95	10.40   --  best one
**CatBoost**	| 36438.77	195.77	0.84	18.90
**XGBoost** | 36259.53	210.66	0.79	14.35
**Random Forest**|	44915.24	230.43	0.70	19.53
**LightGBM**	| 87748.22	312.97	-0.01	60.53



##  Visualizations
The Power BI dashboard includes:
- 2026 Revenue forecast vs 2025 revenue vs 2024 revenue
- Performance comparison of regions and sales representatives with the highest revenue
- Top 10 customers by revenue

##  Business Impact
- **85% forecast accuracy** enables better resource planning
- **60% reduction** in manual data processing time
- **Early warning system** for revenue drops (>10% variance alerts)
- **Data-driven decisions** for commercial strategy

##  Project Structure
```
sales-forecasting-ml/
├── data/
│   ├── raw/                  # Original data files
│   └── processed/            # Cleaned and transformed data
├── notebook/
│   ├── sales_forecasting.ipynb
├── src/
│   ├── data_processing.py   # Data cleaning functions
│   ├── feature_engineering.py
│   └── model_training.py    # Model training pipeline
├── powerbi/
│   └── revenue_dashboard.pbix  # Interactive dashboard
├── features used/
│   └── features_usate.pkl    
├── README.md
├── requirements.txt
└── .gitignore
```



##  Author
**Alessandro Valenti Pettino**
- LinkedIn: www.linkedin.com/in/alessandro-valenti-pettino-b661b4290
- Email: alessandrovalenti2000@gmail.com
- Location: Basel, Switzerland

## License
This project is for portfolio purposes.

# Power BI
 **Note:** `.pbix` file available on request (contains sensitive data)



