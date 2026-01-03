
# Project Background
The objective of this project is to identify high-value customers and customers at risk of churn using RFM (Recency, Frequency, Monetary) analysis. By transforming raw sales data into actionable customer segments, this project helps businesses understand purchasing behavior and prioritize retention and growth strategies. The analysis segments customers into groups such as Champions, Loyal Customers, Potential Loyalists, and At-Risk Customers, enabling data-driven decision-making.


Insights and recommendations are provided on the following key areas:

From a data analyst’s perspective, the business faces a common challenge: while large volumes of sales data are available, there is limited visibility into customer value, loyalty, and churn risk. Marketing and sales teams require actionable insights to answer key questions such as:

- Who are our most valuable customers?
- Which customers are showing signs of disengagement?
- Where should retention and upsell efforts be focused?

To address these questions, RFM (Recency, Frequency, Monetary) analysis is applied to transform raw transactional data into meaningful customer segments that directly support business decision-making 



# Key Analysis Areas

- Insights and recommendations are provided across the following dimensions:
- Customer Value Segmentation – Identifying high-value and low-value customers
- Customer Engagement & Retention – Understanding loyalty and churn risk
- Revenue Contribution – Evaluating which segments drive the majority of sales
- Sales Trends & Performance – Monitoring YoY performance and behavioral shifts

The DAX calculations and data modeling logic used for this analysis are documented within the Power BI model. An interactive Power BI dashboard was developed to explore customer behavior, trends, and segment-level performance.

# Data Structure & Initial Checks

The dataset used in this project is a transaction-level sales dataset, where each row represents an individual customer order. The primary data source includes the following key fields:

Customer ID / Customer Name – Unique customer identifiers
Order ID – Used to calculate purchase frequency
Order Date – Used to calculate customer recency
Product Category – Office Supplies, Furniture, Technology
Sales – Monetary value of each transaction
Quantity, Discount, Profit – Supporting commercial metrics

To enable time-based analysis and proper modeling, a Date Dimension Table was created, containing:

Year, Month, Quarter
Year-Month combinations
Week and Day attributes
Before analysis, the data was validated for:
Missing or invalid dates
Duplicate customer and order records
Consistent customer identifiers

The transactional data was then aggregated at the customer level to calculate Recency, Frequency, and Monetary values.

[Entity Relationship Diagram here]



# Executive Summary

### Overview of Findings

This analysis reveals that a relatively small portion of customers drive a disproportionate share of total revenue, while a significant number of customers fall into low-engagement or at-risk segments. Although overall sales show strong year-over-year growth, declining recency and flat frequency metrics indicate emerging retention risks.

From a stakeholder perspective (Marketing & Sales teams), the three most important takeaways are:

- Champions and Loyal Customers are the primary revenue drivers and should be protected through targeted retention strategies.
- At-Risk and Lost customers represent a measurable churn risk and reactivation opportunity.
- Customer engagement metrics (recency and frequency) require proactive monitoring despite positive sales growth.

[Visualization, including a graph of overall trends or snapshot of a dashboard]



# Insights Deep Dive
### Category 1: Customer Segmentation Distribution

* **Main insight 1.** Champions and Loyal Customers form a strong core customer base. These segments show high purchase frequency and strong monetary contribution, indicating consistent engagement and brand loyalty.
* **Main insight 2.** The largest segment falls under ‘Others’. This group represents average customers with moderate engagement, offering opportunities for upsell and conversion into higher-value segments.
* **Main insight 3.** At-Risk customers make up a meaningful share of the base. These customers were previously active but show declining recency, signaling churn risk.
* **Main insight 4.** Lost customers are a smaller segment but indicate historical churn patterns. Early intervention could prevent further leakage.
[Visualization specific to category 1]


### Category 2: Sales & Revenue Performance

* **Main insight 1.** Total sales reached approximately $613K, reflecting strong overall performance.
* **Main insight 2.** Year-over-Year sales growth of ~30% indicates positive business momentum.
* **Main insight 3.** Revenue growth is uneven across customer segments, with Champions and Big Spenders contributing disproportionately.
  
* **Main insight 4.** High sales growth combined with weakening engagement metrics suggests growth is driven more by spend per customer than by repeat behavior.

[Visualization specific to category 2]


### Category 3: Customer Engagement (Recency & Frequency)

* **Main insight 1.** Average Recency has increased, indicating customers are taking longer between purchases compared to last year.
  
* **Main insight 2.** Average Frequency remains largely flat, suggesting limited improvement in repeat purchase behavior.
  
* **Main insight 3.** Champions maintain strong recency and frequency scores, while At-Risk customers show sharp deterioration.
* **Main insight 4.** Engagement metrics act as early warning indicators, even when revenue performance appears healthy.
[Visualization specific to category 3]


### Category 4: Product Category Contribution

* **Main insight 1.** Office Supplies generate the highest number of customers, indicating broad appeal and frequent purchases.
  
* **Main insight 2.** Technology products contribute higher monetary value per customer, aligning closely with Big Spender and Champion segments.
* **Main insight 3.** Furniture shows moderate engagement, presenting cross-sell opportunities.
* **Main insight 4.** Customer value varies significantly by category, highlighting the importance of category-specific strategies.
[Visualization specific to category 4]



# Recommendations:

Based on the analysis, the following actions are recommended for Marketing and Sales teams:

* Prioritize retention campaigns for Champions and Loyal Customers through personalized offers and loyalty programs**
* Launch reactivation initiatives for At-Risk customers, focusing on time-bound discounts or targeted messaging.**
* Leverage high-value categories (Technology) to upsell mid-tier customers into higher-value segments..**
* Monitor Recency and Frequency KPIs regularly to identify early signs of disengagement.**
* Use customer segmentation to personalize marketing strategies, rather than applying one-size-fits-all campaigns.**
  


# Assumptions and Caveats:

Throughout the analysis, the following assumptions were made:
* Assumption 1 Customers were uniquely identified using Customer ID; duplicate names were treated as separate customers if IDs differed.
  
* Assumption 2 Transactions with valid order dates were included; records with invalid or missing dates were excluded.
  
* Assumption 3 RFM scoring was based on relative ranking (1–5 scale), meaning segment definitions are contextual to this dataset and may shift with new data.

# Conclusion :

This project demonstrates how RFM analysis transforms raw transactional data into a strategic customer intelligence tool. By combining robust data modeling, DAX calculations, and interactive visualization, the dashboard enables stakeholders to quickly identify who drives value, who is at risk, and where to act.

The approach is scalable and can be extended with predictive churn modeling, lifetime value estimation, or campaign performance tracking in future iterations.




<img width="1326" height="739" alt="Image" src="https://github.com/user-attachments/assets/6f2523aa-d1ab-448c-a348-2da11433a70e" />
