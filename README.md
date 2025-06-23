# Analyzing-and-Forecasting-Healthcare-Access-in-Ethiopia-Using-World-Bank-Data
Healthcare Access Analysis and Forecasting in Ethiopia
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg) ![Python](https://img.shields.io/badge/Python-3.8%2B-blue) ![Plotly Dash](https://img.shields.io/badge/Plotly%20Dash-Interactive%20Visualizations-green)
Overview
This project analyzes and forecasts healthcare access in Ethiopia using World Bank data, focusing on key indicators such as health expenditure per capita, physician density, and hospital bed availability. Through exploratory data analysis (EDA), comparative analysis with peer countries (Kenya, Uganda, Rwanda), and time series forecasting with ARIMA models, the project uncovers trends, identifies disparities, and predicts future healthcare metrics. An interactive Plotly Dash dashboard visualizes the findings, and actionable recommendations align with Ethiopia’s Health Sector Transformation Plan (HSTP II) and Sustainable Development Goal 3 (Good Health and Well-being).
Objectives
Analyze Trends: Identify trends in Ethiopia’s healthcare access metrics (2000–2023).

Comparative Analysis: Compare Ethiopia’s metrics with Kenya, Uganda, and Rwanda.

Forecasting: Predict healthcare access metrics for 2024–2028 using ARIMA models.

Visualization: Develop an interactive Plotly Dash dashboard to showcase trends, comparisons, and forecasts.

Policy Recommendations: Provide data-driven insights to support universal health coverage in Ethiopia.

Data Sources
World Development Indicators (WDI): Health expenditure per capita, life expectancy, population metrics.

Health Nutrition and Population Statistics (HNP): Physician density, hospital beds per 1,000 people.

Access: World Bank Open Data (WDI, HNP).

Methodology
Data Cleaning:
Handled missing values with linear interpolation.

Removed outliers using the IQR method.

Normalized data for cross-country comparisons.

Exploratory Data Analysis (EDA):
Univariate analysis: Descriptive statistics and time series plots.

Bivariate analysis: Correlation between expenditure and outcomes.

Multivariate analysis: Principal Component Analysis (PCA).

Comparative Analysis:
Compared Ethiopia with Kenya, Uganda, and Rwanda using bar charts and scatter plots.

Predictive Modeling:
Used ARIMA models for forecasting health expenditure, physician density, and hospital beds.

Evaluated with RMSE and MAE metrics.

Dashboard Development:
Built with Plotly Dash for interactive visualizations of trends, comparisons, and forecasts.

Key Findings
Trends (2000–2023):
Health expenditure per capita improved from -1.56 (2000) to -0.46 (2023).

Physician density rose from 0.021 to 0.108; hospital beds from 0.28 to 0.42.

Life expectancy increased from 52.8 to 66.7 years.

Comparative Insights:
Ethiopia lags Rwanda and Kenya in hospital beds but matches Uganda in physician density.

Forecasts (2024–2028):
Slow growth in health expenditure projected without policy interventions.

Recommendations
Increase health expenditure, inspired by Rwanda’s community-based insurance model.

Expand medical training programs, following Kenya’s approach.

Invest in rural hospital infrastructure to reduce disparities.

Use forecasts to guide resource allocation in HSTP II.

Project Structure

├── data/
│   ├── raw/                     
│   ├── processed/               
├── notebooks/
│   ├── Health Care Access.ipynb 
├── src/
│   ├── data_cleaning.py        
│   ├── analysis.py             
│   ├── modeling.py            
│   ├── dashboard.py           
├── static/
│   ├── visualizations/          
├── README.md                    
├── requirements.txt            
                    
Installation
Clone the repository:
bash

git clone https://github.com/your-username/healthcare-access-ethiopia.git
cd healthcare-access-ethiopia

Install dependencies:
bash

pip install -r requirements.txt

Download World Bank data:
Access datasets from WDI and HNP.

Place raw data in data/raw/.

Run the dashboard:
bash

python src/dashboard.py

Open http://127.0.0.1:8050 in your browser to view the dashboard.

Dependencies
Python 3.7+

Key libraries: pandas, numpy, statsmodels, numpy, plotly, dash, matplotlib, seaborn, sk-learn

Full list in requirements.txt

Usage
EDA: Run notebooks/Health Care Access.ipynb for data exploration and visualizations.

Modeling: Use notebooks/Health Care Access.ipynb to train and evaluate ARIMA models.

Dashboard: Execute src/dashboard.py to launch the interactive dashboard.

Data Processing: Modify src/Health Care Access.ipynb for custom preprocessing.

Results
Visualizations: Interactive time series, bar charts, and scatter plots available in the dashboard.

Model Performance: ARIMA forecasts evaluated with RMSE and MAE, ensuring reliable predictions.

Insights: Ethiopia shows progress but requires increased investment in hospital infrastructure.

Contributing
Contributions are welcome! Please follow these steps:
Fork the repository.

Create a new branch (git checkout -b feature/your-feature).

Commit changes (git commit -m "Add your feature").

Push to the branch (git push origin feature/your-feature).

Open a Pull Request.

Acknowledgments
To dr. Menor for the brilliant lectures and AAU for facilitating the program available to all.
World Bank for providing open-access datasets.

Ethiopia’s Health Sector Transformation Plan (HSTP II) for contextual guidance.

Plotly Dash for enabling interactive visualizations.

Contact
For questions or feedback, reach out to mariyamawittefera@gmail.com or open an issue on GitHub by username @mariyeee
This README is designed to be clear, professional, and engaging. It provides all necessary information for users to understand, install, and contribute to your project.
