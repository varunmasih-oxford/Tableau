# Tableau Assignment: Calculated Fields for Data Analysis

## Objective
In this assignment, you will learn how to create and use Calculated Fields in Tableau to perform real-world data analysis. You will apply mathematical, logical, date, and string functions to uncover insights from sales data.

---

## Skills You Will Practice
- Creating calculated fields in Tableau  
- Using arithmetic and aggregation formulas  
- Applying logical (IF/THEN) conditions  
- Working with dates  
- Using string functions  
- Using calculated fields inside visualizations  

---

## Dataset: Sales_Data.csv

Create a CSV file using the data below and connect it to Tableau.

| Order ID | Order Date | Region | Category | Product Name | Sales | Profit | Quantity | Discount |
|----------|------------|--------|----------|--------------|-------|--------|----------|----------|
| 1001 | 01-01-2024 | East | Furniture | Chair | 12000 | 2000 | 4 | 0.10 |
| 1002 | 05-01-2024 | West | Technology | Laptop | 45000 | 8000 | 2 | 0.05 |
| 1003 | 12-01-2024 | South | Office Supplies | Paper | 3000 | -500 | 10 | 0.20 |
| 1004 | 18-01-2024 | North | Furniture | Table | 15000 | 3000 | 3 | 0.15 |
| 1005 | 25-01-2024 | East | Technology | Printer | 22000 | 4000 | 2 | 0.10 |
| 1006 | 02-02-2024 | West | Office Supplies | Pens | 2000 | 500 | 20 | 0.05 |
| 1007 | 10-02-2024 | South | Technology | Monitor | 18000 | 2500 | 3 | 0.08 |
| 1008 | 14-02-2024 | North | Furniture | Sofa | 30000 | -2000 | 1 | 0.25 |
| 1009 | 20-02-2024 | East | Office Supplies | Binder | 4000 | 800 | 5 | 0.12 |
| 1010 | 28-02-2024 | West | Technology | Mouse | 1500 | 300 | 6 | 0.05 |

---

## Part 1: Data Preparation

1. Connect the dataset to Tableau.  
2. Ensure:
   - Order Date is set as Date  
   - Sales, Profit, Quantity, Discount are set as Measures  
3. Rename fields if necessary for clarity.

---

## Part 2: Basic Mathematical Calculations

Create the following calculated fields:

### Profit Ratio
```

[Profit] / [Sales]

```

### Sales After Discount
```

[Sales] * (1 - [Discount])

```

### Cost Price (Derived)
```

[Sales] - [Profit]

```

### Average Selling Price per Unit
```

[Sales] / [Quantity]

```

---

## Part 3: Logical (IF/THEN) Calculations

### Profit Status
```

IF [Profit] > 0 THEN "Profit"
ELSE "Loss"
END

```

### Sales Category
```

IF [Sales] >= 20000 THEN "High Sales"
ELSEIF [Sales] >= 10000 THEN "Medium Sales"
ELSE "Low Sales"
END

```

### Discount Level
```

IF [Discount] >= 0.20 THEN "Heavy Discount"
ELSEIF [Discount] >= 0.10 THEN "Medium Discount"
ELSE "Low Discount"
END

```

---

## Part 4: Date Calculations

### Order Month Name
```

DATENAME('month', [Order Date])

```

### Order Month Number
```

DATEPART('month', [Order Date])

```

### Order Quarter
```

"Q" + STR(DATEPART('quarter', [Order Date]))

```

---

## Part 5: String Calculations

### Region - Category Label
```

[Region] + " - " + [Category]

```

### Product Description
```

[Product Name] + " | Qty: " + STR([Quantity])

```

---

## Part 6: Build Visualizations Using Calculated Fields

Create the following worksheets:

1. Profit Ratio by Region (Bar Chart)  
2. Sales After Discount by Category (Bar Chart)  
3. Profit vs Loss by Product (Color using Profit Status)  
4. Monthly Sales Trend (Line chart using Order Month Name)  
5. Average Selling Price per Unit by Product  
6. Discount Level by Region (Stacked Bar Chart)

---

## Part 7: Insight-Based Calculated Field

### Performance Category
```

IF [Profit Ratio] > 0.20 THEN "Excellent"
ELSEIF [Profit Ratio] >= 0.10 THEN "Good"
ELSE "Needs Improvement"
END

```

Use this field to:
- Color a bar chart of Products vs Sales  
- Identify which products need attention  

---

## Part 8: Dashboard Creation

Create one dashboard that includes:
- Profit Ratio by Region  
- Monthly Sales Trend  
- Sales After Discount by Category  
- Product Performance Chart  

Add:
- At least one filter  
- Proper titles  
- Legends and labels  

---

## Final Questions

Answer the following:

1. Which region has the highest Profit Ratio?  
2. Which product is being sold with the heaviest discount?  
3. Are high discounts always leading to losses?  
4. Which month shows better overall performance?  
5. Which products fall under Needs Improvement?

