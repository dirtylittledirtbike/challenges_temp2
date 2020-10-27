<!-- # Challenge Set 9
## Part I: W3Schools SQL Lab

*Introductory level SQL*

-- -->

This challenge uses the [W3Schools SQL playground](http://www.w3schools.com/sql/trysql.asp?filename=trysql_select_all). Please add solutions to this markdown file and submit.

1. Which customers are from the UK?
|CustomerID|CustomerName|
|---|---|
4 | Around the Horn
11 | B's Beverages
16 | Consolidated Holdings
19 | Eastern Connection
38 | Island Trading
53 | North/South
72 | Seven Seas Imports

2. What is the name of the customer who has the most orders?

ordercount|CustomerName
--|--
10|Ernst Handel

3. Which supplier has the highest average product price?

|SupplierName|SupplierID|avg_product_price|
|---|---|---|
|Aux joyeux ecclésiastiques|18|263.5|

4. How many different countries are all the customers from? (*Hint:* consider [DISTINCT](http://www.w3schools.com/sql/sql_distinct.asp).)

|Count(Country)|
|---|
|21|

5. What category appears in the most orders?

|count|CategoryName|
---|---
100	| Dairy Products

wait nvm I think i forgot to group by order id first...

|count|CategoryName|
---|---
37|Beverages


6. What was the total cost for each order?

total_price	| CategoryName
--|--
99464.5|Beverages
35071.600000000006|Condiments
54909.16000000001|Confections
69921|Dairy Products
22327.75|Grains/Cereals
51676.52|Meat/Poultry
23401.4|Produce
29652.299999999996|Seafood

7. Which employee made the most sales (by total price)?

 not sure how to answer this will come back
8. Which employees have BS degrees? (*Hint:* look at the [LIKE](http://www.w3schools.com/sql/sql_like.asp) operator.)

EmployeeID|Notes
--|--
3|Janet has a BS degree in chemistry from Boston College). She has also completed a certificate program in food retailing management. Janet was hired as a sales associate and was promoted to sales representative.
5|Steven Buchanan graduated from St. Andrews University, Scotland, with a BSC degree. Upon joining the company as a sales representative, he spent 6 months in an orientation program at the Seattle office and then returned to his permanent post in London, where he was promoted to sales manager. Mr. Buchanan has completed the courses 'Successful Telemarketing' and 'International Sales Management'. He is fluent in French.

Only two!?!

9. Which supplier of three or more products has the highest average product price? (*Hint:* look at the [HAVING](http://www.w3schools.com/sql/sql_having.asp) operator.)

max_avg_price| SupplierName
--|--
46|Tokyo Traders
