# Tableau Sorting & Filtering

## Objective

Learn how to **sort, filter, and explore data** in Tableau to find patterns and simple insights.

---

## Dataset: Superstore Sales (Sample)

| Order ID | Order Date | Region | Category        | Sub-Category | Sales | Profit | Customer Segment |
| -------- | ---------- | ------ | --------------- | ------------ | ----- | ------ | ---------------- |
| 1001     | 01-01-2024 | East   | Furniture       | Chairs       | 450   | 50     | Consumer         |
| 1002     | 03-01-2024 | West   | Technology      | Phones       | 1200  | 300    | Corporate        |
| 1003     | 05-01-2024 | South  | Office Supplies | Binders      | 200   | -20    | Home Office      |
| 1004     | 07-01-2024 | East   | Technology      | Laptops      | 2200  | 500    | Consumer         |
| 1005     | 10-01-2024 | West   | Furniture       | Tables       | 800   | 120    | Corporate        |
| 1006     | 12-01-2024 | North  | Office Supplies | Paper        | 150   | 30     | Home Office      |
| 1007     | 15-01-2024 | South  | Furniture       | Bookcases    | 600   | 80     | Consumer         |
| 1008     | 18-01-2024 | East   | Technology      | Accessories  | 300   | 90     | Corporate        |

Save the file as **superstore_sample.xlsx**

---

# Part A: Tasks (Hands-On)

### Task 1: Sort Categories by Sales

* Drag **Category** → Rows
* Drag **Sales** → Columns
* Sort in **descending order**

### Task 2: Sort Sub-Categories Within Category

* Drag **Sub-Category** under Category
* Sort Sub-Categories by **Profit**

### Task 3: Filter by Region

* Drag **Region** → Filters
* Select **East and West only**

### Task 4: Filter Only Profitable Sales

* Drag **Profit** → Filters → Keep values >= 0

### Task 5: Filter by Date Range

* Drag **Order Date** → Filters → Select **first 10 days of January**

### Task 6: Top N Filter

* Drag **Sub-Category** → Filters → Top → By **Sales** → Top 3

### Task 7: Combined View

* Build a bar chart:

  * Category vs Sales
  * Sorted by Sales descending
  * Filters applied: Region = East, Profit > 0, Top 2 Sub-Categories

---

# Part B: Insightful Questions

1. **Category Performance:** Which category has the most sales? Which has the least? What does this tell you about the business?
2. **Sub-Category Profit:** Which sub-category makes the most profit? Which loses money? Why do you think this happens?
3. **Regional Insights:** After filtering for East and West, which region has higher sales?
4. **Profitable Focus:** When you remove loss-making orders, which products remain? What can this teach you about which products the business should focus on?
5. **Top Products:** Which 3 sub-categories contribute most to total sales? How much of the revenue do they represent?
6. **Date Analysis:** Looking at only the first 10 days of January, do you notice any patterns in sales or profit?
7. **Sales vs Profit:** Are the highest sales items also the most profitable? Identify one example.

---

# Part C: Step-by-Step Instructions

**Sorting:**

1. Click on a field in Rows or Columns.
2. Click the **Sort Ascending** or **Sort Descending** icon.
3. Observe how the chart reorders automatically.

**Filtering:**

1. Drag a field to the **Filters** shelf.
2. Choose the values or range you want to keep.
3. Optionally, right-click → **Show Filter** to make it visible on the sheet.

**Top N Filter:**

1. Drag a dimension to **Filters**.
2. Go to the **Top** tab → Select **By Field** → Enter N → Choose measure (Sales or Profit).

**Combined Filters:**

1. Apply multiple filters together (Region, Profit, Date).
2. Check how sorting and chart appearance change.

---

# Part D: Sample Beginner Insights / Answers

1. **Category Performance:** Technology has the highest sales, Office Supplies has the lowest. This tells us that tech products are driving revenue.
2. **Sub-Category Profit:** Laptops are most profitable; Binders lose money. Possibly due to cost or pricing differences.
3. **Regional Insights:** East region has higher sales than West.
4. **Profitable Focus:** Profitable products include Laptops, Phones, Chairs, Tables. Focus on these for better revenue.
5. **Top Products:** Top 3 sub-categories by sales: Laptops, Phones, Tables. They generate a majority of revenue.
6. **Date Analysis:** In the first 10 days, sales are smaller but Laptops show early high revenue. Could indicate early adopter demand.
7. **Sales vs Profit:** Laptops have high sales and high profit; Phones have high sales but lower profit than Laptops.

---
