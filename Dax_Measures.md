# DAX Measures Used in Global Superstore Analysis

This document contains all DAX Measures created and used in the Power Bi report for Global Superstore dataset. Each measure include a brief explanation.
---
## Total Sales
```DAX
Total sales = SUM(Fact_Table[Sales])
```
### Explanation
Calculates the total revenue generatedfrom all product sales across all orders.

## Total Profit
```DAX
Total Profit = SUM(Fact_Table[Profit])
```
## Total Orders
```DAX
Total Orders = DISTINCTCOUNT(Fact_Table[Order ID])
```
## Average Discount
```DAX
Average Discount = AVERAGE(Fact_Table[Discount])
```
## Average Profit Austrialia
```DAX
AverageProfit_Australia = 
CALCULATE(
     [Average Profit],
    Fact_Table[Country] = "Australia")
```
## Hex Colour
Hex = 
VAR _TopN =
ADDCOLUMNS(
    ALLSELECTED(Fact_Table[Sub-Category]), "Avg Profit", [Average Profit])
    VAR _TopSubcategory = 
    TOPN(1,_TopN,[AverageProfit_Australia],DESC)
    VAR _SelectedSubCategory =
    SELECTEDVALUE(Fact_Table[Sub-Category])
    RETURN
    IF(_SelectedSubCategory IN
    SELECTCOLUMNS(_TopSubcategory,Fact_Table[Sub-Category]), 
    "#12239E",
    "#118DFF")
```
