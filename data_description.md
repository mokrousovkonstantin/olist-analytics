### orders

Order-level dataset containing purchase and delivery timestamps.  
Core table for time-based analysis and delivery performance.

| Column | Description | Usage in Analysis |
|--------|-------------|-------------------|
| order_id | Unique order identifier | Primary key, used to aggregate orders |
| customer_id | Customer identifier | Used to link orders to customers (retention, RFM) |
| order_purchase_timestamp | Purchase datetime | Used for order and revenue trends |
| order_delivered_customer_date | Delivery datetime | Used to calculate delivery time and analyze its impact on customer behavior |

**Derived metrics:**
- delivery_time = delivery date – purchase date  

---

### order_items

Order item-level dataset containing product, seller, and pricing information.  
Main source for revenue and average order value (AOV) calculations.

| Column | Description | Usage in Analysis |
|--------|-------------|-------------------|
| order_id | Unique order identifier | Used to aggregate item-level data to order level |
| order_item_id | Item sequence within order | Used to identify number of items per order |
| product_id | Unique product identifier | Used for category-level and product-level analysis |
| seller_id | Unique seller identifier | Used for regional and seller efficiency analysis |
| price | Item price | Used to calculate revenue and AOV |
| freight_value | Shipping cost | Used to calculate revenue and AOV |

**Derived metrics:**
- revenue = item price + shipping cost 

---

### product

Product-level dataset containing category information.

| Column | Description | Usage in Analysis |
|--------|-------------|-------------------|
| product_id | Unique product identifier | Primary key, used to link products to order_items |
| product_category_name | Product category | Used to analyze category performance and identify high-value segments |

---

### customers

Customer-level dataset used for user behavior and retention analysis.

| Column | Description | Usage in Analysis |
|--------|-------------|-------------------|
| customer_id | Customer identifier | Used to link customers to order_items |
| customer_unique_id | Unique customer identifier | Used for retention and RFM analysis (one user can have multiple orders) |

---

### sellers

Seller-level dataset used for regional and performance analysis.

| Column | Description | Usage in Analysis |
|--------|-------------|-------------------|
| seller_id | Unique seller identifier | Used to analyze seller distribution and revenue per seller |