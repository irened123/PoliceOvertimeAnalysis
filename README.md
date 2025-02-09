# PoliceOvertimeAnalysis  
**A Spark! Project Analyzing Budgetary Allocation and Overtime Spending in the Boston Police Department**  


## **Project Description**  
This project analyzes the Boston Police Department (BPD) budget, focusing on overtime expenditures and financial discrepancies. Given BPD’s $400+ budget, understanding how overtime is allocated is crucial for transparency and accountability. This analysis will examine trends in BPD paychecks, overtime hours paid vs. worked, and discrepancies among officers with lower worked-to-paid ratios to identify potential inefficiencies and anomalies in spending. By uncovering these patterns, this project aims to provide data-driven insights into budget allocation and workforce management.  


## **Key Goals**  

1. **Data Collection & Preprocessing**  
   - Gather and clean BPD employee earnings, overtime records, and budget reports.  
   - Standardize salary and overtime figures, merge datasets, and handle missing values.  

2. **Analyze Budget & Pay Trends**  
   - Examine year-over-year changes in BPD's total budget and overtime allocations.  
   - Compare regular pay vs. overtime pay trends to identify spending patterns.  

3. **Detect Overtime Discrepancies**  
   - Compare overtime hours worked vs. paid to flag inconsistencies.  
   - Identify officers or ranks with disproportionately high overtime pay.  

4. **Data Visualization**  
   - Create time-series plots, heatmaps, and boxplots to highlight spending trends and outliers.  
   - Use histograms and comparative salary distributions to showcase key insights.  

5. **Identify Anomalies & Potential Irregularities**  
   - Apply statistical anomaly detection (Z-scores, IQR) to flag outliers.  
   - Investigate rank, tenure, and department-based discrepancies.  

6. **Forecast Overtime Spending**  
   - Use historical overtime data to predict next year’s expected overtime costs.  
   - Compare projections to BPD’s budget allocation to assess potential overspending.  


## **Data Collection**  

### **Sources**  
The following datasets will be used to analyze BPD employee earnings, overtime trends, and budget allocations:  
- **Employee Earnings Data (2011-2023)**: Contains salary, overtime pay, and total earnings for BPD employees.  
- **Payroll Definitions**: Provides explanations for different payroll categories, including overtime classifications.  
- **BPD Field Activity Data**: Includes records of officer activity, which may help contextualize overtime trends.  
- **BPD Roster Data**: Lists officer ranks, tenure, and department assignments.  
- **BPD Overtime Data (2012-2022)**: Breakdown of overtime hours worked across different categories (court, special events, detail shifts).  
- **2025 City of Boston Operating Budget**: Financial allocations for BPD overtime spending.  

### **Collection Method**  
- **Public government datasets** will be retrieved from official city records.  
- **Overtime data** will be accessed from a provided Google Folder in XLSX format.  
- **CSV and JSON formats** will be used for data preprocessing and merging.  
- **Filtering and aggregation techniques** will be applied to extract relevant police-specific earnings data.  

## **Data Modeling**  

This project will employ statistical analysis and machine learning to identify trends, detect anomalies, and predict overtime spending.  

- **Trend Analysis**: Use time-series models to examine historical overtime spending and budget shifts.  
- **Anomaly Detection**: Apply Z-scores, IQR, and machine learning models (e.g., Isolation Forest) to flag officers with irregular overtime pay.  
- **Overtime Prediction**: Train a regression model (e.g., Linear Regression, Random Forest, XGBoost) to forecast next year’s overtime costs and compare them to budget allocations.  
- **Model Evaluation & Refinement**: Assess model performance using RMSE/MAE, adjust feature selection, and refine based on insights gained during data exploration.  


## **Data Visualization**  
- **Time-Series Analysis**: Track year-over-year trends in overtime spending vs. budget allocation.  
- **Heatmaps**: Highlight departments and officers with disproportionately high overtime.  
- **Boxplots & Histograms**: Compare overtime distributions across ranks and base salaries.  
- **Anomaly Detection**: Flag officers with overtime significantly exceeding department norms.  
- **Scatter Plots**: Visualize overtime hours worked vs. paid to identify discrepancies.  


## **Test Plan**  

To ensure the accuracy and reliability of the analysis, the project will follow a structured testing approach:  

- **Data Splitting**: Withhold 20% of historical overtime data as a test set to evaluate model performance.  
- **Model Validation**: Use cross-validation techniques to prevent overfitting and assess generalizability.  
- **Performance Metrics**: Evaluate predictive models using Root Mean Squared Error (RMSE) and Mean Absolute Error (MAE) to measure accuracy.  
- **Anomaly Detection Assessment**: Compare flagged anomalies against historical trends to validate their significance.  
**

Results will be iteratively refined based on insights from testing, with adjustments made to feature selection, model hyperparameters, and data preprocessing techniques as needed.  


