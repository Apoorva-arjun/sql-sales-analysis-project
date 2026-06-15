# sql-sales-analysis-project

## Objective
SQL analysis of sales performance

## skills used
- SQL
- GitHub

## Findings
- Day 1: SELECT + WHERE + ORDER BY - Top sales by quantity - `IMG_0001.png`
- Day 2: GROUP BY + SUM + LIMIT - Top 5 products by revenue - `IMG_0002.png`
- Day 3: JOIN 2 tables - Show product names instead of IDs - `IMG_0009.png`
- Day 4: JOIN + WHERE - Top 5 products in West region, Laptop = 15k - `IMG_0010.png`
- Day 5: CASE WHEN - Product segmentation. Only Laptop = 'High Value' 15k revenue, all others = 'Low Value' - `IMG_0011.png`
- Day 6: CASE WHEN + WHERE - WEST Region High value products - `IMG_0012.png`
  # SQL Sales Analysis Project - Day 6

## Q1: Highest Revenue Region
Query: SELECT Region, SUM(Sales) AS total_revenue FROM sales GROUP BY Region ORDER BY total_revenue DESC LIMIT 1;
Result: West | 15900
Insight: West region drives 86% of revenue. Focus sales efforts here.`IMG_0013.png`

## Q2: Top 3 Products  
Query: SELECT "Product N...", SUM(Sales) AS total_revenue FROM sales GROUP BY "Product N..." ORDER BY total_revenue DESC LIMIT 3;
Result: Laptop 15000, Desk 2500, Keyboard 900
Insight: Laptop is 83% of total revenue. Prioritize stock/marketing.`IMG_0014.png`

## Q3: Product Value Tiers
Query: [CASE WHEN query you just ran]
Result: High Value 2, Medium Value 1, Low Value 1
Insight: 50% of sales are high-value products. Good revenue mix.`IMG_0015.png`
## Key Insight
Laptop is the #1 product overall and dominates West region revenue. This shows regional product demand varies.
