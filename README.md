# Global_SuperStore

## Table of Content
## project Overview
Global Superstore is a global online retailer based in New York, boasting a broad product catalogue and aiming to be a one-stop-shop for its customers. Global Superstore’s
clientele, hailing from 147 different countries, can browse through an endless offering with more than 10,000 products. 

This large selection comprises three main categories: office supplies (e.g., staples), furniture (e.g., chairs), and technology (e.g., smartphones).
I'm contracted as a Data Analyst to help Global Superstore analyze and draw outmeaningful insight from the Superstore dataset, which would aid management in making informed decisions to improve performance and profitability. 

### Project Objectives
As a data analyst I was tasked with the following
### KPIs
- Total Sales 
- Total Profit 
- Average Discount  
- Total Orders 

### Business Requirement
- Question 1
   - What are the three countries that generated the highest total profit for Global Superstore in 2014?
   - For each of these three countries, find the three products with the highest total profit. Specifically, what are the products’ names and the total profit for each product? 
- Question 2
   - Identify the 3 subcategories with the highest average shipping cost in the United States. 
- Question 3
   - Which city is the least profitable (in terms of average profit) in the United States? For this analysis, discard the cities with less than 10 Orders. 
   - Why is this city’s average profit so low?
- Question 4
   - Which product subcategory has the highest average profit in Australia?
- Question 5
   - Assess Nigeria’s profitability (Total Profit) for 2014. How does it compare to other African countries? 
   - What factors might be responsible for Nigeria’s poor performance? You might want to investigate shipping costs and the average discount as potential root causes. 

### Tools Used & Data Source
- Power BI
   - for data Cleaning
   - Modeling and Visualization
- Data Source: Global Superstore dataset in Microsoft Excel [download here].(https://www.microsoft.com)

### Data Cleaning and Modeling
- Removed irrelevant columns not necessary for my analysis.
- Created a calendar table for time-based analysis.
- Created a separate Measures Table for all DAX calculations

### Measures Used
- All measures used in this analysis can be assessed here [View DAX Measures](./Dax_Measures.md).

### KPI 
- Total sales
-  picture of the total sales 
The measure used. Calculate the total sales across all transactions.

- Total profit
-  picture of the total profit 
The measure used. Calculate the total profit the store actualize after all expenses 

- Average Discount
- picture of the average discount 
The measure used. Calculate the average discount across all products 

- Total Orders
-  picture of the total orders
The measure used. Calculate the total numbers of orders placed by customer 

- Average Shipping cost () picture of the AVG shipping Cost . The measure used. Calculate the AVG. Shipping cost across all providers.

- Total customer 
- picture of the total customer 
The  measure used.Total customer across all the countries

### Bussines Requirement & Insight
1. Top 3 Countries by Profit (2014)

![Top 3 Countries by Profit](https://github.com/Chisom83/Global_SuperStore/blob/main/Image/Screenshot%202025-05-09%20051839.png?raw=true)

- Insight:
   - United States, India and China generated the highest profit in 2014.
   - United States maintained profitability across all years due to a strong customer base.
> Measure used: 

- For each of these countries, the top 3 products by profit were identified using tooltips.
   - Hovering over each country reveals a tooltip showing the top 3 most profitable products in that region for 2014.
  

2. Three subcategories with the highest Average Shipping Cost (USA)

Insight:
   - Heavier products like Copiers, Machines and Tables incur higher shipping costs.
> visualization:

3. Least Average Profitable City in the United States

Insight:
   - Lancaster had low average profit despite that its order is above ten.
   - Cities with discount rates above 0.16 showed reduced profitability and average profitability.
   - High Discount is responsible for there low profit.
> Visualization

4. Highest Average Profit Subcategory in Australia

![Average profit subcategory_Australia](https://github.com/Chisom83/Global_SuperStore/blob/main/Image/Screenshot%202025-05-09%20051856.png?raw=true)

- Insight:
   - Appliances stood out as the most average profitable subcategory.
> Measure used

5. Nigeria's Profitability (2014 vs Other African Countries)

> Visualization: 
Insight:
   - Across 45 African countries that patronize the store, Nigeria has the highest customers and order volume but lowest profit.
   - In order of ranking in total Sales Nigeria ranked the fifth and the least in total profit showing that they are making sales but generating no profit at all.
   - High discount rates is the primary factors leading to low profit.
   - Discounts are applied to every product ordered, which significantly reduces profit margins.
   - shipping costs in Nigeria are relatively moderate, and not a contributing factor to the poor profit performance.
  
### Recommendations
- Temporarily Eliminate Discounts:
   - Remove all product discounts for a three-month trial period, monitor the effect on sales, customer retention, and profit. This will help evaluate whether discounts are essential for maintaining customer activity.

- Adjust Discount Strategy if Necessary:
   - If removing discounts results in a significant drop in customer engagement, reintroduce discounts only on bulk purchases ( e.g.,5 items and above) and ensure that discount rates remain below the average discount rate of the store.
   - Alternatively, offer non-monetary incentives such as free gifts for purchases of five or more different items.
   
### Conclusion

Discounting is a key driver of low profitability despite strong sales. Top-performing markets (e.g., United State, South African in the African region) had minimal or no discounts. Strategic reduction in discounts can significantly improve profit without sacrificing sales volume.

### Dashboard
link to dataset 








 







