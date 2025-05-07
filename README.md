# Global_SuperStore
## Overview
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

### Tools Used
- Power BI
   - for data Cleaning
   - Modeling and Visualization

### Data Cleaning and Modeling
- Removed irrelevant columns not necessary for my analysis.
- Created a calendar table for time-based analysis.
- Created a separate Measures Table for all DAX calculations

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

Insight:
   - United States, India and China generated the highest profit in 2014.
   - United States maintained profitability across all years due to a strong customer base.
> Visualization: 

- For each of these countries, the top 3 products by profit were identified using tooltips.

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

Insight:
   - Appliances stood out as the most profitable subcategory.
> Visualization

5. Nigeria's Profitability (2014 vs Other African Countries)

> Visualization: 
Insight:
   - Across 45 African countries that patronize the store Nigeria, has the highest customers and order volume but lowest profit.
   - In order of ranking in total Sales Nigeria ranked the fifth and the least in total profit showing that they are making sales but not generating profit at all.
   - High discount rates were the primary factors causing the low profitability.
   - Shipping cost is not significant in the cause of low profitability .

### Recommendations

- Reduce or remove discount in underperforming markets like Nigeria.
- Consider non-monetary incentives (e.g., bulk bonus) instead of discounts.
- Apply discounts only to bulk purchases (e.g., 5+ items).
- Conduct a 3-month test period in key markets to monitor impact of reduced discounts.

### Conclusion

Discounting is a key driver of low profitability despite strong sales. Top-performing markets (e.g., United State, South African) had minimal or no discounts. Strategic reduction in discounts can significantly improve profit without sacrificing sales volume.


---








 




Recommendation 
To increase profits in most countries discount should be removed for a trial of three months and see if it will affect the store positively or negatively. In country like Nigeria Which they have already developed a strong market presence removing discount will help covert the customer and high volume in profit. In city, state and country not performing well  discount removals should be looked into.

Discount can also be placed for customer that purchase five goods and above rather than putting discount on each purchase of a goods.

Offer of non monetary offers should be placed on a bulk purchase and discount removed.

The store should not close down but the following recommendation should be put into consideration and see which works more better.

Conclusion 
Form my analysis it's seen that discount is a key factor in low profits generation and high sales. Most countries like UK in general and Sudan in Africa performing well have no discount at all and they're performing greatly so discount should be removed than the store running low profits generation store with other store profit. When applying these steps the should still provide top notch services so that customers will still patronize dispect no discount.
