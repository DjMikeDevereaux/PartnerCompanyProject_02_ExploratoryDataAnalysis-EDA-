°# PartnerCompanyProject_02_ExploratoryDataAnalysis-EDA-
The goal of this Exploratory Data Analysis (EDA) is to understand the weekly sales behavior 
The goal of this Exploratory Data Analysis (EDA) is to understand the weekly sales behavior of the partner company by examining:

-Weekly sales trends
-Regional sales variation
-Identification of high‑ and low‑rotation products
-Relationship between units sold and total sales value
-Preparing the dataset for further analysis (predictive modeling, dashboards, KPIs)

This analysis is part of the Partner Company Project in the EBAC Data Science & Business Analytics program.

## Data Sources Used
1. FACT_SALES.csv
-Contains transactional sales information:
  ° WEEK — Week in XX-YY format
  ° ITEM_CODE — Product code
  ° TOTAL_UNIT_SALES — Units sold
  ° TOTAL_VALUE_SALES — Total sales value
  ° TOTAL_UNIT_AVG_WEEKLY_SALES — Weekly average units sold
  ° REGION — Sales region

2. DIM_CALENDAR.xlsx
Calendar table with:
  -WEEK
  -YEAR
  -MONTH
  -WEEK_NUMBER
  -DATE

## EDA Workflow
1. Data Loading
  Datasets were loaded using pandas:

python
  import pandas as pd
  df_fact = pd.read_csv("FACT_SALES.csv")
  df_cal = pd.read_excel("DIM_CALENDAR.xlsx")

2. Initial Exploration
The notebook examines:
  -Dataset dimensions
  -Data types
  -First rows
  -Sales distribution by region
  -Weekly variation in units and sales value

3. Calendar Integration
Merging with the calendar table enables:
  - Monthly trend analysis
  - Year-over-year comparison
  - Detection of peak and low sales weeks

4. Pattern Identification
The EDA aims to answer questions such as:
  - Which products have the highest rotation?
  - Which regions generate the most sales?
  - How do sales evolve throughout the year?
  - Are there weeks with unusual or extreme sales values?

## Expected EDA Outputs
Depending on your visualizations, this README anticipates:
  - Distribution plots of sales
  - Weekly time series
  - Product rankings by units and value
  - Regional comparisons
  - Business insights derived from the data

## Preliminary Conclusions
- Sales vary significantly across weeks and regions.
- Certain products show strong rotation patterns useful for forecasting.
- Calendar integration reveals monthly and seasonal trends.
- Some weeks show atypical behavior that may require deeper investigation.


