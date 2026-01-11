Superstore Sales Dashboard – Part II

Overview

This project is a continuation of the Superstore Sales Dashboard, focusing on detailed SQL analysis and Power BI dashboards to understand sales, profit, and product-level performance across segments, categories, and regions. The goal is to extract actionable business insights from transactional data and visualize them effectively for decision-making.

The dashboards cover:

Query-01: Monthly sales and profit trends by region

Query-02: Segment and category-level contribution analysis

Query-04: Region vs category performance matrix

Query-05: Product-level profitability, loss exposure, and risk identification

The project demonstrates end-to-end data handling, transformation, visualization, and insight derivation.

-----------------------------------------------------------------------------------------------------------------------------

Problem Statement

Superstore management wants to:

Identify high-performing products and categories

Understand regional and segment contribution to sales and profit

Detect loss-making products and evaluate their impact

Enable informed business decisions for inventory, pricing, and portfolio optimization

The project solves the problem of turning raw transactional data into meaningful KPIs, insights, and visual analytics.
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Concepts & Techniques Used
SQL Concepts

SELECT, SUM, COUNT, LAG, CASE for aggregation and trend analysis

GROUP BY for summarizing data by product, category, segment, and region

Window functions (LAG, RANKX) for previous period comparisons and ranking

Conditional flags (Profit Flag) to identify loss vs profit

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------

Power BI Concepts

Data Import & Modeling from SQL queries

Matrix and Card visuals for product-level and KPI analysis

Clustered Column Charts & Donut Charts for categorical comparisons

Conditional Formatting to highlight losses (red) and profits (green)

Tooltips & Product Codes for clean, readable dashboards with full information

Measures vs Columns for correct aggregation and loss calculation
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

INSIGHTS

DASHBOARD-1 Sales & Profit Performance Overview

1. West and East dominate both sales and profit
•	West cumulative sales: 713.47K → highest by region
•	West cumulative profit: 106.02K
•	East cumulative sales: 672.19K
•	East cumulative profit: 90.67K
Together, West + East contribute ~61% of total sales and ~69% of total profit, highlighting strong regional concentration.
2.  South shows high sales but lower profit contribution
•	South cumulative sales: 388.98K
•	South cumulative profit: 46.04K
Despite decent sales, profit margin is lower (~11.8%), indicating higher costs or lower pricing efficiency compared to West and East.
3.  Profitability does not always follow sales growth
•	Central cumulative sales: 497.80K
•	Cumulative profit: 40.13K
•	Furniture in Central shows negative profit (–2.59K)
Highlights that high sales do not guarantee high profit, and certain products/regions require cost control.
4.  Monthly performance shows peaks and troughs
•	Highest sales month: November 2017 → 117.38K
•	Lowest profit month: January 2015 → –3.29K
Indicates seasonality and profit volatility, suggesting need for strategic planning during low-profit months.


DASHBOARD-02 Revenue & Profit Insights by Segments

5. Consumer segment drives the most sales
The Consumer segment contributes ~50.7% of total sales, making it the largest revenue driver, followed by Corporate (~30.7%) and Home Office (~18.6%).
6.  Profit is highly concentrated in Technology and Office Supplies
Technology contributes ~51.4% of total profit, Office Supplies ~42.6%, and Furniture only 6%, showing that over 94% of profits come from just two categories.
7. Furniture is a weak performer
Furniture contributes the least to profit (~6%) despite moderate sales, highlighting low margins or high cost pressure in this category.
8.  Profit vs sales efficiency
Some segments like Consumer have high sales but moderate profit, while Technology and Office Supplies achieve higher profit margins relative to sales, indicating better pricing and cost management.

DASHBOARD-03 Sales & Profit Analysis by Category


9. Technology leads sales but profit varies by region
•	Technology is the top-selling category with 835.9K (~36.8% of total sales).
•	East region Tech profit (47.44K) slightly exceeds West (44.27K) despite similar sales, highlighting regional differences in profitability.

10.  Furniture underperforms in certain regions
•	Furniture in Central region reports a negative profit of –2.59K, indicating margin issues despite moderate sales.
•	Other regions show low-to-moderate Furniture profit, emphasizing the category’s weak contribution to overall profit.

11.  Sales do not always translate to high profit
•	West Furniture: 248K sales → 10.59K profit (~4.3% margin)
•	Central Tech: 170K sales → 33.69K profit (~19.8% margin)
This demonstrates that profitability is more efficient in Tech and Office Supplies, not necessarily in high-sales categories like Furniture.

12. Profit concentration in West and East regions
•	West and East regions together account for ~70% of total profit, highlighting dependence on these regions for overall profitability.

13. Office Supplies show strong margins despite moderate sales
•	West OS: 213K sales → 51.16K profit (~24% margin)
•	East OS: 202K sales → 40.73K profit (~20% margin)
Indicates efficient operations and good pricing strategy for Office Supplies.

DASHBOARD-04 
Product Profit Overview with loss flags

14. Loss prevalence vs impact
•	291 products are loss-making, indicating that a large portion of the product portfolio is unprofitable.
•	However, the total loss amount is only –76.50K, compared to an overall total profit of 282.86K.
Insight:
While many products operate at a loss, their financial impact is limited, suggesting losses are spread thinly rather than concentrated in a few high-risk products.

15. Profit concentration
•	Despite widespread product losses, the business remains net profitable.
•	Profits are driven by a smaller subset of high-performing products, which more than offset losses.
Insight:
Overall profitability is dependent on a limited number of strong products, highlighting the importance of protecting and scaling top performers.

16. Optimization opportunity (key business takeaway)
•	The high count of loss-making products suggests:
o	Pricing inefficiencies
o	Cost overruns
o	Low-volume SKUs
Insight:
Rationalizing or improving underperforming products could significantly improve margins without harming total sales.




