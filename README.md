# Retail Sales Analysis Dashboard

## Objective
Analyze retail sales data to identify top revenue-generating products, 
best-performing regions, most profitable customer segments, and monthly 
sales trends.

## Tools Used
Excel, SQL (SQLite & MySQL), Power BI

## Dataset
Sample Superstore Dataset (Kaggle)

## Business Questions
1. Which products generate maximum revenue?
2. Which regions perform best?
3. Which customer segments are most profitable?
4. What are the monthly sales trends?
5. Who are the top customers, and which categories underperform on profit?

## Key Insights

### From Excel Analysis
- Canon imageCLASS 2200 Advanced Copier is the top revenue product ($61.6K)
- West region leads in both sales and profit
- Consumer segment is the most profitable
- Sales grew from $484K (2014) to $733K (2017)

### From SQL Analysis
- Identified top 10 customers by revenue and profit contribution
- Found specific sub-categories with the weakest profit performance, 
  highlighting where discounting or cost issues may be hurting margins
- Built a monthly revenue trend with month-over-month change using a 
  CTE and window function (LAG)

### From Power BI Dashboard
- West region leads in both revenue and profit, while Central shows 
  weaker profit relative to its sales volume, suggesting margin pressure
- Consumer segment drives 47% of total profit, nearly 1.5x more than 
  Corporate and over 2x Home Office
- Revenue shows a clear seasonal pattern, dipping at the start of most 
  years before recovering, with growth accelerating sharply through 
  2016-2017
- A single product accounts for more than double the revenue of the 
  next highest product, showing heavy reliance on a small number of 
  high-ticket items

## SQL Analysis
Queries were written and tested in both **SQLite** (DB Browser) and 
**MySQL** (MySQL Workbench) to demonstrate adaptability across SQL 
dialects. Both versions are available in `/sql-queries/`.

Techniques used: GROUP BY, aggregations (SUM, ROUND), CTEs, and window 
functions (LAG).

## Power BI Dashboard
Built an interactive dashboard featuring:
- KPI cards: Total Revenue, Total Profit, Total Orders, Profit Margin
- Revenue trend by quarter (2014-2017)
- Region-wise revenue and profit comparison
- Top 10 products by revenue
- Customer segment profit breakdown
- Written business insights embedded directly in the dashboard

File available in `/powerbi-file/`.

## Repository Structure

## Repository Structure
```
