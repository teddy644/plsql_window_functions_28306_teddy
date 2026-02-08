# plsql_window_functions_28306_teddy


## Business Problem

### Business Context

Camellia Restaurant is a mid-sized restaurant operating in the food service industry. The management wants to better understand customer behavior, product performance, and sales trends to support data-driven decision-making.

### Data Challenge

Camellia Restaurant collects transactional sales data daily, but the data has not been fully analyzed to extract meaningful insights. Management struggles to identify top-performing menu items, customer purchasing patterns, and sales trends over time.

### Expected Outcome

The analysis aims to provide actionable insights that help management improve menu optimization, customer targeting, and revenue growth.

---

## Success Criteria

The project achieves the following five measurable goals using SQL window functions:

1. Identify the **top 5 menu items per month** using `RANK()`
2. Calculate **running monthly sales totals** using `SUM() OVER()`
3. Measure **month-over-month sales growth** using `LAG()`
4. Segment customers into **quartiles based on spending** using `NTILE(4)`
5. Compute **three-month moving average sales trends** using `AVG() OVER()`

---

## Database Schema Design

```
sql

```
### ER Diagram
![ER](screenshots/ER_diagram.png)

## Part A: SQL JOINs Implementation

### JOIN Types Implemented

1. **INNER JOIN** – Retrieve transactions with valid customers and products
2. **LEFT JOIN** – Identify customers who have never made a transaction
3. **RIGHT JOIN / FULL JOIN** – Detect products with no sales activity
4. **FULL OUTER JOIN** – Compare customers and products including unmatched records
5. **SELF JOIN** – Compare customers within the same region

Each JOIN includes:

* Well-commented SQL query
* Screenshot of query results
* 2–3 sentence business interpretation

---

## Part B: SQL Window Functions Implementation

### Window Function Categories

#### 1. Ranking Functions

* `ROW_NUMBER()`
* `RANK()`
* `DENSE_RANK()`
* `PERCENT_RANK()`
  **Use case:** Top-performing products and customers by revenue

#### 2. Aggregate Window Functions

* `SUM()`, `AVG()`, `MIN()`, `MAX()`
* Both `ROWS` and `RANGE` frames applied
  **Use case:** Running totals and sales trends

#### 3. Navigation Functions

* `LAG()`, `LEAD()`
  **Use case:** Month-over-month sales comparison

#### 4. Distribution Functions

* `NTILE(4)`, `CUME_DIST()`
  **Use case:** Customer segmentation

Each function includes:

* SQL query with comments
* Screenshot of results
* Interpretation (2–3 sentences)

---

## Results Analysis

### Descriptive Analysis

Sales performance varies by month and product category, with specific menu items consistently generating higher revenue.

### Diagnostic Analysis

Seasonal trends and customer purchasing frequency significantly influence monthly revenue fluctuations.

### Prescriptive Analysis

Camellia Restaurant should promote high-performing menu items, introduce loyalty programs for high-value customers, and adjust inventory planning based on sales trends.

---

## Key Insights

* A small number of menu items generate a large share of total revenue
* High-value customers can be effectively segmented using spending quartiles
* Sales trends reveal opportunities for targeted promotions

---

## References

* Oracle SQL Documentation
* PostgreSQL Window Functions Documentation
* Academic SQL tutorials and course materials

---

## Academic Integrity Statement

“All sources were properly cited. Implementations and analysis represent original work. No AI-generated content was copied without attribution or adaptation.”

---

## Author

**Name:** [Your Full Name]
**Student ID:** [Your Student ID]
**Group:** [Your Group]
