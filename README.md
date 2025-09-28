### Customer-Financial-Data-Insights-Dashboard

## Project Overview
  This project aims to perform a comprehensive analysis of a financial loan dataset using SQL queries and Power BI visualisations. The analysis focuses on understanding loan performance trends, funding patterns, payment behaviour, and borrower demographics to deliver actionable business insights.
The dataset includes detailed loan information such as loan amounts, interest rates, borrower income, loan purpose, loan status, repayment amounts, and demographic attributes (e.g., employment length, home ownership, and address state).

## Objectives
 - Analyse loan performance over time and by borrower characteristics.
 - Assess month-to-date (MTD) and previous month-to-date (PMTD) loan trends.
 - Examine funding amounts and repayment rates.
 - Identify performing vs non-performing loans and understand their distribution.
 - Evaluate loan patterns by purpose, term, grade, and borrower profile.
 - Provide insights for financial risk management and strategic decision-making.

## Methodology
# Data Preparation with SQL Server
 - Data preparation is the first step of the analysis. SQL was used to:
 - Connect to the database and extract relevant tables such as loans, borrower details, repayment schedules, and loan status.
 - Clean and structure data by removing duplicates, handling missing values, and ensuring consistent formats.
 - Aggregate transactional data to create monthly and quarterly summaries for performance analysis.
 - The SQL process ensures that the imported data in Power BI is optimised for reporting and analysis.
   
# Data Modelling in Power BI
Once the cleaned data was imported into Power BI, a relational data model was created to link relevant datasets efficiently. Relationships were defined between loan data, borrower details, and time-based tables. This structure enables dynamic filtering and aggregation in dashboards.
Key considerations in data modelling included:
 - Maintaining a central fact table for loan transactions.
 - Establishing dimension tables for borrower information, loan details, and time attributes.
 - Optimising model performance by eliminating unnecessary columns and ensuring correct relationship directions.
   
# Date Table Creation
A date table is essential in Power BI for time intelligence calculations. In this project, a dedicated date table was created with attributes such as year, month, quarter, and week. This allows for seamless time-based analysis, such as month-over-month comparisons or year-to-date metrics.
The date table was marked as the official Date Table in Power BI, ensuring all time calculations function correctly.

# Measure Creation with DAX
DAX (Data Analysis Expressions) was used to create dynamic measures to enhance reporting. Measures included:
 - Total Loan Amount – calculates the sum of all loans within a selected period.
 - Month-to-Date and Year-to-Date Calculations – track loan performance over time.
 - Loan Performance Ratios – such as the percentage of performing loans compared to total loans.
 - Average Interest Rates – to monitor borrower cost trends.
 - These measures allow stakeholders to filter data interactively and view real-time insights.

# Dashboard Development
The final stage was designing an interactive dashboard in Power BI to present the insights clearly. Dashboard features included:
 - Time-based loan application and repayment trends.
 - Comparative analysis of performing vs non-performing loans.
 - Loan amounts segmented by borrower demographics and loan purpose.
 - KPIs and visual cards to highlight key metrics at a glance.
 - Interactivity was enhanced through slicers and filters, allowing decision-makers to explore data from different perspectives.

# Key Insights
 - Seasonal patterns in loan applications were observed, with peaks in certain months.
 - Borrower profiles and loan purposes influence repayment rates significantly.
 - Clear trends in performing loans can guide risk management strategies.
   
# Tools & Technologies
- SQL – Data extraction, cleaning, and preparation.
- Power BI – Data modelling, date table creation, DAX measure creation, and visualisation.
- DAX – Creating business-critical measures for dynamic reporting.

# Potential Applications
 - Enhanced credit risk assessment.
 - Loan product design based on borrower behaviour and repayment patterns.
 - Automated reporting for financial decision-making and forecasting.
