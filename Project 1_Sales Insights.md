**Part-5: Build Dashboard** 

***29. Verify through SQL: 
SQL Code: 
SELECT sum(transactions.sales_amount)
FROM sales.transactions
INNER JOIN sales.date
ON transactions.order_date = date.date 
Where date.year = 2020 and date.month_name = "January"
AND (transactions.currency = 'INR\r' OR transactions.currency = "USD\r"); 

*** The answer matches exactly with Power BI results




***30. Show revenue by region.
Just select the market_name and drag it to the y axis. Same, do for the sales quantity. 



***31. Verify SQL for Chennai's Total revenue or sales quantity.
Select SUM(transactions.sales_amount)
FROM sales.transactions
INNER JOIN sales.date
ON transactions.order_date = date.date
where date.year = 2020 AND transactions.market_code = "MARK001";




***32. Show top 5 customers in Power BI.
Go to "Filter" section and select what you need. 



***33. If you want to show the customer's name in full, just increase the Y axis MAX AREA WIDTH.

![image](https://github.com/zizanayub/Sales-Insights-and-Dashboard_Power-BI/assets/65456659/4e23e922-5033-42bd-ade0-49ccbda37017)




***34. Find the top 5 products just how we found top 5 customers. 

![image](https://github.com/zizanayub/Sales-Insights-and-Dashboard_Power-BI/assets/65456659/ce7fb555-e7fb-4149-871f-2112be398f9d)




***35. Make a revenue trend of last 4 years. It's wasy. Just do it by your own.

![image](https://github.com/zizanayub/Sales-Insights-and-Dashboard_Power-BI/assets/65456659/a60a04e3-6d53-4b70-963b-f7dc8f974d6a)







**<u>Part-06 (Stakeholders Feedback)</u>**


***01.Problem Solution: Only show relevant data visualization.
Suppose you selected a company named Nixon and it's showing different portions of different bar charts. Which looks clumsy and unclear. 


![image](https://github.com/zizanayub/Power-BI-Projects/assets/65456659/dcb59067-c871-4c26-839f-93a816d1bea3)


We need only the relevant bars.What we can do?

<u>Solution:</u> 
Go to File >> Options and Settings >> Options >> Current File >> Report Settings >> Check "Change Default Visual Interaction from cross highlighting to 
cross filtering" 
