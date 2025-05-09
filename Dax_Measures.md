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
## Total Quantity
```DAX
Total Quantity = SUM(Fact_Table[Quantity])
```
## Average Discount
```DAX
Average Discount = AVERAGE(Fact_Table[Discount])
```
## Total Customers
```DAX
Total Customers = DISTINCTCOUNT(Fact_Table[Customer ID])
```
## Average Shipping Cost
```DAX
Average Shipping Cost = AVERAGE(Fact_Table[Shipping Cost])
```
## Average Profit Austrialia
```DAX
AverageProfit_Australia = 
CALCULATE(
     [Average Profit],
    Fact_Table[Country] = "Australia")
```
## Hex Colour
```DAX
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
## Average Shipping Cost USA
```DAX
AverageShippingCost_USA = 
CALCULATE(
     [Average Shipping Cost],
    Fact_Table[Country] = "United States"
)
```
## Average Profit Per City
```DAX
AvgProfitPerCity = 
IF([TotalOrdersPerCity] >=10, 
DIVIDE([TotalProfitPercity],[TotalOrdersPerCity]),
BLANK()
)
```
## Total Africa Customers
```DAX
AfricaTotalCustomers = CALCULATE([Total Customers],Fact_Table[Region] = "Africa")
```
## Total Africa Sales
```DAX
AfricaTotalSales = 
CALCULATE([Total sales], Fact_Table[African Country] = "Africa")
```
## Total Africa Profit
```DAX
AfricaTotalProfit = 
CALCULATE([Total Profit], Fact_Table[African Country] = "Africa")
```
## Average Africa Discount
```DAX
AfricaAvgDiscount = 
CALCULATE([Average Discount], Fact_Table[African Country] = "Africa")
```
## Africa Total Quantity
```DAX
AfricaTotalQuantity = 
CALCULATE([Total Quantity], Fact_Table[African Country] = "Africa")
```
## Africa Total Orders
```DAX
AfricaTotalOrders = CALCULATE([Total Orders], Fact_Table[African Country] = "Africa")
```
## Africa Total Shipping Cost
```DAX
AfricaTotalShippingCost = 
CALCULATE([Total Shipping Cost],Fact_Table[African Country] = "Africa")
```
