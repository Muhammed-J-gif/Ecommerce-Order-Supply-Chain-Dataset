# Business Requirements Gathering for BI Reports

## 1. Identifying Key Stakeholders
This report is intended for **technical recruiters and employers** to review.  
It is formatted like a **consumer‑style report** to make project findings easy to navigate.

---

## 2. Defining Reporting "Objectives"
The dataset is hosted on **Kaggle**, and the original business objective is not explicitly defined.  
For this project, the analysis focuses on understanding operational and sales performance.

### Business Objectives
- Improve order fulfillment efficiency  
- Understand customer purchasing behavior  
- Monitor sales performance across products, categories, and regions  
- Identify logistics bottlenecks (shipping delays, delivery failures)  
- Evaluate supplier performance and inventory flow  
- Reduce operational costs in the supply chain  

### Additional Operational Focus (Chosen for This Project)
Viewing the dataset as a **stationary operations monitoring system**:
- Daily order volume  
- Real‑time delivery status  
- Warehouse queue and backlog 
- Carrier delays  

---

## 3. Identify Key Performance Indicators (KPIs)

### KPIs
- Total revenue (price + shipping charges)  
- Average order value (Total Revenue ÷ Number of Orders) 
- On‑time delivery rate  (Calculation TBD)
- Customer lifetime value (CLV) (CLV = Total Revenue per Customer)
- Payment success rate  (Payment Success Rate = Number of Successful Payments / Total Payment Attempts)
- Category‑level sales  ()

### Operational KPIs
- Daily order volume  
- Delivery status tracking  
- Warehouse backlog  --- Additional data is required from wharehouse to measure the backlog of orders.
- Carrier performance  --- Additional data is required from wharehouse to measure the operation of order fulfillment.

---

## 4. Gather Data Requirements

All required data is already included in the dataset:

| Table | Key Fields |
|-------|------------|
| **Orders** | timestamps, status |
| **Order Items** | price, shipping, product, seller |
| **Customers** | location |
| **Payments** | payment type, value |
| **Products** | category, dimensions |

### Granularity
The dataset includes timestamps, enabling:
- Trend analysis  
- Seasonality analysis  
- Cohort analysis  

---

## 5. Identify Report Structure & Visualization Needs

### Reporting Format Options
- **Dashboards** (interactive, high‑level)  
- **Static reports** (PDF/Excel exports)  
- **Self‑service BI tools** (Power BI, Tableau, Looker)

### Visualization Types
- Bar charts  
- Line charts  
- Pie charts  
- Heatmaps  
- KPI indicators  

### Filters & Drill‑Downs
- Date range  
- Product category  
- Customer region  
- Delivery status  

---

## 6. Document Business Rules & Calculations

### Data Transformations
- Currency normalization (Not required due to the data already display sale price without currency symbols. This helps with keep the nurmerical data consistent as EDA is done.)
- Timestamp conversions  
- Delivery time calculations  

### Calculated Fields
- Revenue growth rate  
- Customer churn rate  
- Delivery delay duration  

### Aggregation Rules
- SUM (revenue, quantity)  
- AVG (order value, delivery time)  
- MEDIAN (shipping cost)  

