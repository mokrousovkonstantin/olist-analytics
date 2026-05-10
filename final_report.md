# E-commerce Growth Analysis: Retention, AOV and Revenue Concentration (Olist)

## Objective

The goal of this analysis is to find revenue growth opportunities in an e-commerce business.

---

## Key Findings

### 1. Revenue growth is driven by volume, not efficiency

Revenue peaked at 1,2M in Nov 2017, driven by order growth (>7k), while AOV remained flat (150 – 175).

![Count orders Trend](figures/01_Number_of_orders_by_month.png)

![Revenue Trend](figures/02_Revenue_by_month.png)

![Average bill Trend](figures/03_Average_bill_by_month.png)

**Conclusion:** Revenue growth is driven purely by increasing order volume, while average order value remains flat. This indicates that growth is not scalable, as it depends solely on acquiring more orders rather than increasing revenue per order.

---

### 2. Strong dependence of sales on SP state.

The concentration of sales volume and value by region is highly concentrated in SP state (38% of total sales and 41% of total orders). Therefore, the business is highly dependent on this region. The gap with the region in 2nd and 3rd place is three times. Also, the distribution of states by sales volume almost completely matches the distribution of states by number of orders.

![Sales distribution by states](figures/07_Distribution_of_sales_by_state.png)

![Number of orders distribution by states](figures/08_Distribution_of_the_number_of_orders_by_state.png)

**Conclusion:** The high revenue share of SP state is achieved through scale (number of sellers and orders), not through efficiency.

Low revenue per seller in SP state is due to:
1. High competition between sellers
2. A decrease in the average order value

The opposite situation is observed in other regions: fewer sellers and orders, but higher average order value and revenue per seller. This indicates oversaturation of the SP state market and underutilized growth potential in other regions.

**Business Implication:** High dependence on a single region creates concentration risk and limits sustainable growth.

---

### 3. Customer retention is critically low

The average number of orders per customer is 1,03, indicating that the vast majority of users make only a single purchase.

![Orders per unique customer Trend](figures/12_Number_of_orders_per_unique_customer_by_month.png)

**Interpretation:**
The business generates minimal repeat sales and is highly dependent on continuous customer acquisition for revenue growth.

**Customer Segmentation (RFM Analysis):**

- One-time customers dominate the user base:
  - more than 77% of customers (active + dormant)
  - more than 76% of total revenue

- Loyal customers represent a negligible share:
  - <1% of users
  - <2% of revenue

- High-value (VIP) customers:
  - about 1% of users
  - about 2,4% of revenue

Implication:
With 77% one-time customers, even a small increase in repeat rate (e.g. +10%) could significantly increase revenue without additional acquisition costs.

**Key Drivers:**

- **Product categories do not explain retention**  
  Repeat purchase rates are consistent across categories (1,0 – 1,1 orders per customer)

- **Delivery time impacts customer activity**  
  Faster delivery regions show higher engagement, while regions with delivery times >15 days show lower activity

**Conclusion:**
Customer retention is structurally weak, with no stable base of repeat customers.  
Delivery time is a key lever that can potentially improve customer behavior and increase repeat purchases.

---

### 4. Revenue is highly concentrated in high-value orders

High-value orders are disproportionately concentrated in specific product categories.

Top categories such as:
- relogios_presentes (2,6x)
- consoles_games (2,3x)
- beleza_saude (1,8x)

are significantly overrepresented in the top 5% of orders compared to their baseline share.

This indicates that certain categories have a much higher likelihood of generating high-value transactions.

**Conclusion:**
Product category is a key driver of high-value orders. A small group of categories contributes disproportionately to high-revenue transactions.


## Recommendations

### 1. Fix customer retention
- Focus on one-time customers (77% of user base) as the primary growth lever
- Trigger reactivation campaigns within 30 – 60 days after first purchase
- Prioritize high-value one-time customers for retention efforts
- Develop strategies to convert one-time buyers into repeat customers
- Even a +0,1 increase in orders per customer could lead to 10% revenue growth

---

### 2. Logistics optimization
- Prioritize logistics improvements in regions with delivery times >15 days, as these regions show lower customer activity
- Estimate potential uplift by comparing order frequency with regions delivering within 7–10 days

---

### 3. Scale high-value categories
- Promote high-value products through homepage placement and recommendation blocks
- Expand assortment in high-value categories
- Use upsell and recommendation systems
- Focus on categories contributing to top 5% high-value orders

---

### 4. Reduce dependency on SP
- Expand seller base in high AOV regions (RS, RJ, SC, PR)
- Shift marketing spend outside SP

---

### 5. Increase AOV in SP
- Introduce bundles
- Promote premium alternatives
- Use recommendation blocks


## Next Steps

### 1. Validate retention drivers
- Perform cohort analysis to measure retention over time  
- Quantify the impact of delivery time on repeat purchase probability  
- Identify behavioral differences between one-time and repeat customers  

---

### 2. Deep dive into high-value orders
- Analyze the composition of top 5% orders (categories, price ranges, customer segments)  
- Identify whether high-value orders are driven by one-time or repeat customers  
- Estimate potential scenarios for increasing average order value (AOV)  

---

### 3. Regional expansion analysis
- Evaluate market potential in non-SP states (RS, RJ, SC, PR)  
- Compare customer acquisition efficiency and revenue contribution across regions  
- Identify priority regions for scaling seller acquisition  

---

### 4. Customer segmentation refinement
- Build deeper customer segmentation beyond RFM (behavioral or value-based clusters)  
- Identify high-potential segments for retention and upsell  
- Quantify revenue contribution by each segment  

---

### 5. Experiment design
- Define A/B tests for:
  - retention campaigns  
  - delivery speed improvements  
  - AOV growth strategies (bundles, recommendations)  
- Define success metrics and estimate expected business impact  