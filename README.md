# E-commerce Revenue Analysis (Olist)

## Goal
Identify key drivers of revenue growth and structural limitations (retention, AOV, regional dependency)

## What Was Done
- Data cleaning and preprocessing
- Data mart creation (SQL + pandas)
- Exploratory data analysis (EDA)
- RFM customer segmentation
- Hypothesis testing (retention, AOV, regional effects)

## Key Insights
- Revenue growth is driven by order volume, not AOV (flat at 150 – 175)
- Customer retention is critically low (1,03 orders per customer)
- Revenue is highly concentrated: top 5% of orders generate 34%
- Business is heavily dependent on SP state (38% revenue)

## Business Impact
- Growth depends on new customers - high CAC risk  
- No stable revenue base  
- Untapped potential in non-SP regions  

## Project Structure
- /data/raw — not included in repository
- /data/processed — cleaned data  
- /notebooks — analysis  
- /figures — visualizations  
- final_report.md — business conclusions  

## Tools
Python (pandas, matplotlib), SQL
