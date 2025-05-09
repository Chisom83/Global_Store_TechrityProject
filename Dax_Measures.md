# DAX Measures Used in Global Superstore Analysis

This document contains all DAX Measures created and used in the Power Bi report for Global Superstore dataset. Each measure include a brief explanation.
---
## Total Sales
```DAX
Total sales = SUM(Fact_Table[Sales])
```
### Explanation
Calculates the total revenue generatedfrom all product sales across all orders.
