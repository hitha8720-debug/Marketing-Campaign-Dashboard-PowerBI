# Marketing Campaign Dashboard — Power BI

## Objective
Analysed 2,200+ customer records to evaluate marketing campaign 
performance, customer segmentation, and spending behavior using 
Power BI and DAX.

## Tools Used
Power BI Desktop, DAX (Data Analysis Expressions), Power Query

## Dataset
Kaggle — iFood Marketing Data (2,200+ customer records)

## Dashboard Pages

### Page 1 — Campaign Overview
- KPI cards: Total Customers (2K), Total Revenue (1M), Avg Spend 
  per Customer (562.76), Avg Customer Income (51.62K), Campaign 
  Response Rate (15%)
- Spend by Customer Segment (High / Mid / Low Value)
- Revenue Share by Product Category

### Page 2 — Campaign Performance
- Campaign acceptance comparison across 5 campaigns
- Response rate by Education level
- Response rate by Marital Status

## Key Findings
- High Value customers generate ₹0.75M in spend versus just ₹0.09M 
  from Low Value customers — revenue is heavily concentrated in a 
  small top-tier segment.
- Wine is the dominant product category, contributing 50.45% of 
  total revenue, followed by Meat Products at 27.24%.
- Customers with a Graduation-level education respond to campaigns 
  far more than other education levels, with response dropping 
  sharply for Master's, PhD, and Basic education segments.
- Campaign 2 significantly underperformed compared to Campaigns 
  1, 3, 4, and 5 — accepted by only 4.55% of responders versus 
  21–25% for the others, flagging it as a candidate for review or 
  redesign.
- Single and Married customers show the highest campaign response 
  rates, while Widowed customers respond the least.

## DAX Measures Used
- Total Revenue = SUM(MntTotal)
- Total Customers = COUNTROWS
- Campaign Response Rate = DIVIDE(Response, Total Customers)
- Avg Customer Income = AVERAGE(Income)
- Avg Spend per Customer = DIVIDE(Total Revenue, Total Customers)
- Customer_Segment = Calculated column classifying customers into 
  High / Mid / Low value tiers based on total spend

## Files
- Marketing_Campaign_Dashboard.pbix — full Power BI file
- Screenshots — dashboard preview images
