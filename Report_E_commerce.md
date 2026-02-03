## Part 1: Data Preparation

### Task 1: Connect & Verify Data

1. Connect the dataset to Tableau.
2. Ensure:

   * **Order Date** and **Ship Date** are set as **Date type**
   * **Shipping Delay** is numeric
3. If Shipping Delay is not provided, create a calculated field:

```
Shipping Delay = DATEDIFF('day', [Order Date], [Ship Date])
```

---

## Part 2: Shipping Performance Analysis

### Task 2: Average Shipping Delay by Ship Mode

Create a bar chart showing:

* **Ship Mode** on Rows
* **AVG(Shipping Delay)** on Columns

**Question to Answer:**
Which shipping mode is the slowest?

---

### Task 3: Monthly Shipping Trend

Create a line chart:

* **Order Date (Month)** on Columns
* **AVG(Shipping Delay)** on Rows

**Insight Goal:**
Are delays increasing during certain months?

---

### Task 4: On-Time vs Delayed Orders

1. Create a calculated field:

```
Delivery Status
IF [Shipping Delay] <= 2 THEN "On Time"
ELSE "Delayed"
END
```

2. Build a pie chart:

   * **Delivery Status** on Color
   * **COUNT(Order ID)** on Angle/Label

**Question:**
What percentage of orders are delayed?

---

## Part 3: Customer & Segment Insights

### Task 5: Delay by Customer Segment

Create a bar chart:

* **Segment** on Rows
* **AVG(Shipping Delay)** on Columns

**Business Question:**
Which customer segment experiences the most delays?

---

### Task 6: Top 10 Customers with Highest Delays

1. Put **Customer Name** on Rows
2. Put **AVG(Shipping Delay)** on Columns
3. Sort descending
4. Add a **Top 10 filter** by AVG(Shipping Delay)

**Insight Goal:**
Which customers are most affected by slow shipping?

---

## Part 4: Order Volume vs Delay

### Task 7: Orders Over Time

Create an area or line chart:

* **Order Date (Month)** on Columns
* **COUNT(Order ID)** on Rows

**Question:**
Do more orders lead to higher delays?

---

### Task 8: Relationship Between Order Volume & Delay

Create a scatter plot:

* **MONTH(Order Date)** on Detail
* **COUNT(Order ID)** on Columns
* **AVG(Shipping Delay)** on Rows

**Insight Goal:**
Is there a correlation between high order volume and shipping delays?

---

## Part 5: Dashboard Creation

### Task 9: Build a Management Dashboard

Create a dashboard containing:

1. Average Delay by Ship Mode
2. Monthly Delay Trend
3. Delay by Segment
4. On-Time vs Delayed Pie Chart
5. Top 10 Delayed Customers

### Add Interactivity

Add filters for:

* Ship Mode
* Segment
* Order Date (Year)

---

## Part 6: Final Business Questions (Answer in a Short Report)

Students must answer:

1. Which shipping mode should the company improve first?
2. During which months are delays highest?
3. Which customer segment faces the most shipping issues?
4. Are delays linked to higher order volumes?
5. What operational improvement would you suggest?

---
