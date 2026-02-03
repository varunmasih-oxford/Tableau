# Data Visualization Guide: Chart Types, When to Use Them

Understanding which chart to use is essential for clear and effective data storytelling. This guide explains common chart types, when to use them, and real-world examples.

---

## 1. Bar Chart

**Best for:** Comparing values across categories
**Use when:** You want to show differences between groups or rankings.

**Examples:**

* Sales by Product Category
* Number of Students in Each Course
* Average Shipping Delay by Ship Mode

---

## 2. Column Chart

**Best for:** Comparing categories over time (short time periods)
**Use when:** Time-based comparison with fewer periods (months, quarters).

**Examples:**

* Monthly Revenue for Q1
* Orders per Month (Jan–Jun)

---

## 3. Line Chart

**Best for:** Showing trends over time
**Use when:** You want to track increases, decreases, or patterns across continuous time.

**Examples:**

* Website Traffic Over a Year
* Monthly Shipping Delay Trend
* Stock Price Movement

---

## 4. Area Chart

**Best for:** Showing trends over time with emphasis on volume
**Use when:** You want to show magnitude of change over time.

**Examples:**

* Total Sales Growth Over Years
* Number of Orders Processed Monthly

---

## 5. Pie Chart

**Best for:** Showing proportions of a whole
**Use when:** You have a small number of categories (ideally fewer than 5).

**Examples:**

* Market Share by Brand
* Percentage of On-Time vs Delayed Orders

---

## 6. Donut Chart

**Best for:** Same as pie chart, with space for labels in the center
**Use when:** You want to show proportions with a modern look.

**Examples:**

* Budget Distribution by Department

---

## 7. Stacked Bar Chart

**Best for:** Comparing totals and sub-categories together
**Use when:** You want to see both overall value and composition.

**Examples:**

* Sales by Region split by Product Category
* Orders by Segment split by Ship Mode

---

## 8. Stacked Area Chart

**Best for:** Showing part-to-whole trends over time
**Use when:** You want to track how categories contribute to totals over time.

**Examples:**

* Revenue by Product Line Over Years

---

## 9. Scatter Plot

**Best for:** Showing relationship between two numeric variables
**Use when:** You want to identify correlation, clusters, or outliers.

**Examples:**

* Advertising Spend vs Sales
* Order Volume vs Shipping Delay

---

## 10. Bubble Chart

**Best for:** Comparing three numeric variables
**Use when:** You want to add size as a third dimension.

**Examples:**

* Sales vs Profit with Bubble Size = Quantity Sold

---

## 11. Histogram

**Best for:** Showing distribution of a single numeric variable
**Use when:** You want to understand frequency ranges.

**Examples:**

* Distribution of Delivery Delays
* Student Exam Score Distribution

---

## 12. Box Plot (Box-and-Whisker Plot)

**Best for:** Showing spread and outliers in data
**Use when:** You want to compare distributions across groups.

**Examples:**

* Shipping Delay by Ship Mode
* Salary Distribution by Department

---

## 13. Heat Map

**Best for:** Showing patterns using color intensity
**Use when:** You want to compare values across two dimensions.

**Examples:**

* Sales by Month and Region
* Website Activity by Day and Hour

---

## 14. Tree Map

**Best for:** Showing hierarchical part-to-whole data
**Use when:** You want to show proportions across many categories.

**Examples:**

* Sales by Category and Sub-Category

---

## 15. Map Chart

**Best for:** Geographic data visualization
**Use when:** Location plays an important role in analysis.

**Examples:**

* Sales by State or Country
* Orders by Region

---

## 16. Gantt Chart

**Best for:** Project timelines
**Use when:** You want to track task durations and schedules.

**Examples:**

* Project Implementation Plan
* Marketing Campaign Timeline

---

## 17. Waterfall Chart

**Best for:** Understanding how a starting value is affected by increases and decreases
**Use when:** You want to show step-by-step contribution to a total.

**Examples:**

* Revenue Breakdown (Revenue → Costs → Profit)

---

## 18. Funnel Chart

**Best for:** Showing stages in a process
**Use when:** You want to visualize drop-offs between steps.

**Examples:**

* Sales Funnel (Leads → Prospects → Customers)
* Website Conversion Funnel

---

## Quick Chart Selection Guide

| Goal                         | Best Chart Type      |
| ---------------------------- | -------------------- |
| Compare categories           | Bar / Column Chart   |
| Show trend over time         | Line / Area Chart    |
| Show proportions             | Pie / Donut Chart    |
| Show distribution            | Histogram / Box Plot |
| Show relationship            | Scatter Plot         |
| Show geographic data         | Map                  |
| Show part-to-whole hierarchy | Tree Map             |
| Show process stages          | Funnel Chart         |
| Show project schedule        | Gantt Chart          |

---



# Sample Datasets for Different Chart Types


## 1. Compare Categories — Bar / Column Chart

**Use Case:** Compare performance across different groups.

| Product Category | Sales Amount |
| ---------------- | ------------ |
| Electronics      | 15000        |
| Furniture        | 12000        |
| Clothing         | 9000         |
| Grocery          | 7000         |

---

## 2. Show Trend Over Time — Line / Area Chart

**Use Case:** Track changes over time.

| Month | Orders |
| ----- | ------ |
| Jan   | 120    |
| Feb   | 150    |
| Mar   | 170    |
| Apr   | 160    |
| May   | 190    |
| Jun   | 210    |

---

## 3. Show Proportions — Pie / Donut Chart

**Use Case:** Show parts of a whole.

| Segment     | Customers |
| ----------- | --------- |
| Consumer    | 500       |
| Corporate   | 300       |
| Home Office | 200       |

---

## 4. Show Distribution — Histogram / Box Plot

**Use Case:** Understand spread of numeric values.

| Delivery Delay (Days) |
| --------------------- |
| 1                     |
| 2                     |
| 2                     |
| 3                     |
| 3                     |
| 4                     |
| 5                     |
| 6                     |
| 7                     |
| 8                     |

---

## 5. Show Relationship — Scatter Plot

**Use Case:** Identify correlation between two variables.

| Advertising Spend ($) | Sales ($) |
| --------------------- | --------- |
| 1000                  | 5000      |
| 1500                  | 7000      |
| 2000                  | 9000      |
| 2500                  | 10000     |
| 3000                  | 12000     |

---

## 6. Show Geographic Data — Map Chart

**Use Case:** Compare values by location.

| State      | Sales |
| ---------- | ----- |
| California | 15000 |
| Texas      | 12000 |
| Florida    | 9000  |
| New York   | 11000 |
| Illinois   | 8000  |

---

## 7. Show Part-to-Whole Hierarchy — Tree Map

**Use Case:** Show contribution of sub-categories within categories.

| Category    | Sub-Category | Sales |
| ----------- | ------------ | ----- |
| Electronics | Phones       | 8000  |
| Electronics | Laptops      | 7000  |
| Furniture   | Chairs       | 5000  |
| Furniture   | Tables       | 4000  |
| Clothing    | Men          | 4500  |
| Clothing    | Women        | 4500  |

---

## 8. Show Process Stages — Funnel Chart

**Use Case:** Track drop-off in a process.

| Stage            | Users |
| ---------------- | ----- |
| Website Visitors | 5000  |
| Product Views    | 3500  |
| Add to Cart      | 2000  |
| Checkout Started | 1200  |
| Purchases        | 800   |

---

## 9. Show Project Schedule — Gantt Chart

**Use Case:** Visualize task timelines.

| Task                 | Start Date | End Date  |
| -------------------- | ---------- | --------- |
| Requirement Analysis | 01-Jan-24  | 05-Jan-24 |
| Design Phase         | 06-Jan-24  | 12-Jan-24 |
| Development          | 13-Jan-24  | 25-Jan-24 |
| Testing              | 26-Jan-24  | 31-Jan-24 |
| Deployment           | 01-Feb-24  | 03-Feb-24 |



