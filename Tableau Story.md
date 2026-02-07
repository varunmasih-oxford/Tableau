# Tableau Story

## Practice Dataset: Retail Sales Performance

Copy the data below into Excel and save it as **retail_sales.csv**, then connect it to Tableau.

| Order Date | Region | Category        | Sub-Category | Sales | Profit | Segment     |
| ---------- | ------ | --------------- | ------------ | ----- | ------ | ----------- |
| 01-01-2025 | North  | Furniture       | Chairs       | 1200  | 200    | Consumer    |
| 05-01-2025 | South  | Technology      | Phones       | 2200  | 500    | Corporate   |
| 12-01-2025 | East   | Office Supplies | Binders      | 800   | 120    | Home Office |
| 18-01-2025 | West   | Furniture       | Tables       | 1500  | -200   | Consumer    |
| 25-01-2025 | North  | Technology      | Laptops      | 3000  | 700    | Corporate   |
| 02-02-2025 | South  | Office Supplies | Paper        | 600   | 80     | Home Office |
| 10-02-2025 | East   | Furniture       | Bookcases    | 1100  | 150    | Consumer    |
| 14-02-2025 | West   | Technology      | Accessories  | 900   | -50    | Corporate   |
| 20-02-2025 | North  | Office Supplies | Pens         | 400   | 60     | Home Office |
| 28-02-2025 | South  | Furniture       | Chairs       | 1300  | 250    | Consumer    |
| 05-03-2025 | East   | Technology      | Phones       | 2100  | 450    | Corporate   |
| 11-03-2025 | West   | Office Supplies | Storage      | 700   | -100   | Consumer    |

---

## Story Objective

**Business Question:**
Which region and product category are causing low profitability?

This story guides users from high-level performance to detailed problem areas.

---

## PART 1: Create Worksheets

### Sheet 1: KPI Overview

Steps:

1. Drag **Sales** to Text
2. Drag **Profit** to Text
3. Change Marks type to **Text**
4. Format numbers clearly

Purpose: Overall sales and profit summary.

---

### Sheet 2: Sales by Region

Steps:

1. Drag **Region** to Rows
2. Drag **Sales** to Columns
3. Sort in descending order
4. Show data labels

Purpose: Identify top-performing regions by sales.

---

### Sheet 3: Profit by Region

Steps:

1. Drag **Region** to Rows
2. Drag **Profit** to Columns
3. Drag **Profit** to Color
4. Use color to differentiate profit and loss

Purpose: Identify loss-making regions.

---

### Sheet 4: Profit by Category

Steps:

1. Drag **Category** to Rows
2. Drag **Profit** to Columns
3. Drag **Profit** to Color

Purpose: Compare profitability across categories.

---

### Sheet 5: Sub-Category Loss Details

Steps:

1. Drag **Sub-Category** to Rows
2. Drag **Profit** to Columns
3. Sort ascending (loss at top)

Purpose: Identify exact products causing losses.

---

## PART 2: Create Tableau Story

Click **New Story** in Tableau and select an appropriate size.

---

### Story Point 1: Overall Company Performance

Sheet Used: KPI Overview

Title:
Overall Sales Are Good, But Profit Needs Attention

Insight:
Introduces the overall business performance.

---

### Story Point 2: Sales Performance by Region

Sheet Used: Sales by Region

Title:
North and South Lead in Sales

Insight:
Sales appear strong across regions.

---

### Story Point 3: Profit Analysis by Region

Sheet Used: Profit by Region

Title:
West Region Is Making Loss

Insight:
Profit reveals issues not visible in sales alone.

---

### Story Point 4: Category-Level Analysis for West

Steps:

1. Open Profit by Category sheet
2. Filter **Region = West**
3. Add filtered view to Story

Title:
Furniture and Technology Are Weak in the West

Insight:
Narrow down the problem categories.

---

### Story Point 5: Sub-Category Drill Down

Steps:

1. Open Sub-Category Loss sheet
2. Filter **Region = West**
3. Add to Story

Title:
Tables and Storage Are Driving the Loss

Insight:
Pinpoint exact sub-categories causing losses.

---

### Story Point 6: Final Recommendation

Text-only Story Point

Title:
Final Business Recommendation

Content:

* West region is unprofitable
* Furniture (Tables) and Office Storage items are main loss drivers
* Suggested actions:

  * Reduce discounts
  * Review costs and suppliers
  * Adjust pricing strategy

---

