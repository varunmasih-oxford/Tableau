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

## CONTAINS

### Check if String Contains Text

```tableau id="39bgfu"
CONTAINS("Calculation", "alcu")
```

### Result

```text id="7wybd6"
TRUE
```

---

## ENDSWITH

### Check String Ending

```tableau id="h9t7c0"
ENDSWITH("Tableau", "leau")
```

### Result

```text id="n0g5vi"
TRUE
```

---

## FIND

### Find Position of Text

```tableau id="4zvqkn"
FIND("Calculation", "alcu")
```

### Result

```text id="0k9b7o"
2
```

---

## FINDNTH

### Find Nth Occurrence Position

```tableau id="4wnr6r"
FINDNTH("Calculation", "a", 2)
```

### Result

```text id="iqk9q0"
7
```

---

## LEFT

### Extract Left Characters

```tableau id="jlwm9s"
LEFT("Matador", 4)
```

### Result

```text id="jlwm9t"
Mata
```

---

## LEN

### Count String Length

```tableau id="jlwm9u"
LEN("Matador")
```

### Result

```text id="jlwm9v"
7
```

---

## LOWER

### Convert Text to Lowercase

```tableau id="jlwm9w"
LOWER("ProductVersion")
```

### Result

```text id="jlwm9x"
productversion
```

---

## LTRIM

### Remove Leading Spaces

```tableau id="jlwm9y"
LTRIM(" Matador ")
```

### Result

```text id="jlwm9z"
Matador 
```

---

## MAX

### Find Maximum Value

```tableau id="8jp6n1"
MAX(4, 7)
```

### Result

```text id="8jp6n2"
7
```

---

## MID

### Extract Middle Characters

```tableau id="8jp6n3"
MID("Calculation", 2, 5)
```

### Result

```text id="8jp6n4"
alcul
```

---

## MIN

### Find Minimum Value

```tableau id="8jp6n5"
MIN(4, 7)
```

### Result

```text id="8jp6n6"
4
```

---

## PROPER

### Convert Text to Proper Case

```tableau id="8jp6n7"
PROPER("PRODUCT name")
```

### Result

```text id="8jp6n8"
Product Name
```

---

## REPLACE

### Replace Text in String

```tableau id="8jp6n9"
REPLACE("Version 3.8", "3.8", "4x")
```

### Result

```text id="8jp6na"
Version 4x
```

---

## RIGHT

### Extract Right Characters

```tableau id="8jp6nb"
RIGHT("Calculation", 4)
```

### Result

```text id="8jp6nc"
tion
```

---

## RTRIM

### Remove Trailing Spaces

```tableau id="8jp6nd"
RTRIM(" Calculation ")
```

### Result

```text id="8jp6ne"
 Calculation
```

---

## SPACE

### Generate Spaces

```tableau id="8jp6nf"
SPACE(2)
```

### Result

```text id="8jp6ng"
  
```

---

## SPLIT

### Split String into Parts

```tableau id="8jp6nh"
SPLIT("a-b-c-d", "-", 2)
```

### Result

```text id="8jp6ni"
b
```

---

## STARTSWITH

### Check String Beginning

```tableau id="8jp6nj"
STARTSWITH("Matador", "Ma")
```

### Result

```text id="8jp6nk"
TRUE
```

---

## TRIM

### Remove Leading and Trailing Spaces

```tableau id="8jp6nl"
TRIM(" Calculation ")
```

### Result

```text id="8jp6nm"
Calculation
```

---

## UPPER

### Convert Text to Uppercase

```tableau id="8jp6nn"
UPPER("Calculation")
```

### Result

```text id="8jp6no"
CALCULATION
```

---



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

