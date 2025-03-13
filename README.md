
# MIST 4610 - Project 1 - Group 7:




## Team Name:
- 61608 Group 7
## Team Members:

- Allmond, Chandler [@Chandler Allmond](https://github.com/chandlerallmond)
- Barton, Nick [@Nick Barton](https://github.com/nicholasbarton1)
- Manav Kamdar [@Manav Kamdar] (https://github.com/manavk2004)
- Sengaphone, Vincent [@Vincent Sengaphone](https://github.com/sengaphone)
- Wilson, Landon [@Landon Wilson](https://github.com/landonnn0)

## Problem Description:

Retail technology businesses, such as Best Buy, face challenges in efficiently managing inventory, sales transactions, and product categorization. Without an organized database system, these businesses may encounter difficulties such as:
- Overstocking or understocking due to poor inventory tracking.
- Inefficient sales tracking, leading to unclear insights on employee performance and product demand.
- Difficulty in categorizing products, which slows down retrieval and impacts customer service.
- Lack of visibility into sales trends, making it harder for management to optimize stock levels and pricing strategies.

To address these challenges, the Electronic Product Database is designed as a comprehensive inventory and sales tracking system. This database will:
- Store detailed product information, including descriptions, pricing, warranty periods, and brand associations.
- Track real-time inventory status, restock dates, and reorder quantities.
- Facilitate sales transactions, recording employee sales contributions, transaction amounts, and payment methods.
- Enable sales analysis, allowing management to identify top-selling products, evaluate employee performance, and forecast future demand.

By implementing this database, businesses can improve inventory accuracy, sales efficiency, and data-driven decision-making to enhance overall operations.

## Data Model:

The Electronic Product Database is designed to manage the inventory and sales of an electronics retail business. This data model provides a structured way to store and retrieve information about electronic products, their availability, and their categorization. The electronic_product table serves as the core of the model, linking products to their respective brands and categories through the brand_name and type_of_device tables. Additionally, the inventory table ensures that stock levels and restocking requirements are efficiently tracked, preventing shortages and optimizing supply chain operations.

The sales transaction process is handled through the sales_transaction and sales_transaction_product tables, which record transaction details, payment methods, and the number of products sold. Each sale is associated with an employee, stored in the employee table, allowing management to track individual employee contributions to sales. This structure ensures that every transaction is linked to both the products being sold and the employees processing the sales, making it easier to evaluate performance and analyze revenue trends.

By integrating inventory, sales, and employee management, this database provides businesses with real-time insights into product performance, stock availability, and financial transactions. The structured relationships between tables allow for streamlined data retrieval, enabling managers to make data-driven decisions regarding restocking, sales strategies, and employee performance evaluations. This system ultimately helps improve operational efficiency, profitability, and customer satisfaction by ensuring that products are always available and transactions are accurately recorded.

<img width="900" alt="Screenshot 2025-03-13 at 12 21 56 PM" src="https://github.com/user-attachments/assets/fd30e664-1276-4929-ad69-98a52e26c572" />

## Data Dictionary:
<img width="900" alt="Screenshot 2025-03-13 at 12 23 33 PM" src="https://github.com/user-attachments/assets/1c8b02df-ea89-462f-a8c7-c347bd8bb99c" />

<img width="900" alt="Screenshot 2025-03-13 at 12 24 07 PM" src="https://github.com/user-attachments/assets/196067c9-c487-4d52-a7e7-5e63b3deb49e" />

<img width="900" alt="Screenshot 2025-03-13 at 12 24 44 PM" src="https://github.com/user-attachments/assets/d2aba09a-718f-4ed5-81c6-2361936d80d5" />

<img width="900" alt="Screenshot 2025-03-13 at 12 25 12 PM" src="https://github.com/user-attachments/assets/90e710fc-a6a0-4faa-944d-d0d2d779908e" />

<img width="900" alt="Screenshot 2025-03-13 at 12 25 50 PM" src="https://github.com/user-attachments/assets/4ee88f02-8aea-48d8-b4ad-1d6a984d4713" />

<img width="900" alt="Screenshot 2025-03-13 at 12 26 08 PM" src="https://github.com/user-attachments/assets/d5afeb49-4003-46a0-a751-ebdf3b549c6b" />

<img width="900" alt="Screenshot 2025-03-13 at 12 26 30 PM" src="https://github.com/user-attachments/assets/53edb716-5441-4c87-875b-ad372fb2bc76" />

## Queries:
1. Low Stock & High Stock Alert
This query identifies products with low stock levels and high stock levels to help businesses manage inventory efficiently. The low stock alert retrieves products with a stock quantity of 30 or less, ensuring that managers restock them before they run out. The high stock alert retrieves products with a stock quantity greater than 50, helping managers avoid excessive inventory that could lead to high storage costs or markdowns. Both queries order the results in ascending order of stock quantity for better visibility.
 <img width="900" alt="Screenshot 2025-03-13 at 12 28 22 PM" src="https://github.com/user-attachments/assets/9825fb50-3228-4f51-ac76-0a7f42b22c4a" />
Managers can use this query to maintain balanced stock levels by ensuring that fast-selling products are restocked in time while preventing overstocking of slow-moving items. This helps businesses reduce waste, improve cash flow, and optimize inventory space, leading to better profitability and operational efficiency.
2. Best Selling Products
This query retrieves the top 5 best-selling products based on the total quantity sold. The results are sorted in descending order by sales volume.
<img width="900" alt="Screenshot 2025-03-13 at 12 30 11 PM" src="https://github.com/user-attachments/assets/a70d252a-a1b5-4138-991b-bebf90b33eee" />
Managers can identify high-demand products, allowing them to prioritize restocking and promotional efforts.
3. Total Revenue By Product Category
This query calculates the total sales revenue for each product category while filtering out categories that generate less than the average revenue of all categories. It first groups transactions by product category to compute total revenue and then applies a HAVING clause to retain only those categories that exceed the average revenue. A subquery is used to determine the overall average category revenue, ensuring that the analysis focuses on high-performing product categories.
<img width="900" alt="Screenshot 2025-03-13 at 12 49 01 PM" src="https://github.com/user-attachments/assets/346ad81c-0651-4170-bef2-df8ba2ae3542" />
Managers can use this query to identify high-performing product categories that generate above-average revenue. By filtering out lower-performing categories, businesses can allocate more resources to profitable categories, optimize inventory planning, and adjust marketing strategies for better financial outcomes.
4. Top 3 Most Profitable Brands
If a store wanted to maximize revenue by stocking the brands from which consumers were purchasing most from, this code would be beneficial to visualize which brands sat at the top of the revenue chart.
<img width="900" alt="Screenshot 2025-03-13 at 12 30 55 PM" src="https://github.com/user-attachments/assets/85e5a732-629e-4bcb-be0c-ebb76f3cb26f" />
The code joins the sales transaction, sales transaction for products, electronic product, and brand name tables then groups it by brand name then order by total revenue. Then we set the limit to 3 in order to show only the top 3 brands by revenue.
5. Employee Preformance
Shows each of the employee’s sales performance and gives basic information including their name and employee id
<img width="900" alt="Screenshot 2025-03-13 at 12 31 13 PM" src="https://github.com/user-attachments/assets/34a14eab-c2d0-4500-8977-781249cee2f1" />
Managers can use this to gauge whether employees are meeting the standards that the company has set for itself. Having a clear and concise table showing the level of performance each employee brings into the company can allow managers to pinpoint those who may need extra assistance, and give the proper guidance for success. Comparing the performance of each employee overtime can allow the managers to make logical decisions to keep employees, fire employees, give bonuses, etc.
6. Monthly Sales Trends
This query displays the year, month, and total sales revenue for each month. The results are grouped by month and sorted in descending order to show the most recent months first.
<img width="900" alt="Screenshot 2025-03-13 at 12 31 41 PM" src="https://github.com/user-attachments/assets/0e9249d5-c9d2-4f36-8515-767167509958" />
Managers can use this query to analyze sales trends over time, identifying seasonal patterns and peak sales months. This insight helps businesses make data-driven decisions about inventory management, pricing strategies, and marketing campaigns to maximize revenue.
7. Total Sales Transactions
This query retrieves the total number of transactions in the system.
<img width="900" alt="Screenshot 2025-03-13 at 12 31 59 PM" src="https://github.com/user-attachments/assets/a6e407a2-d051-4a28-8ffc-964a32515420" />
Gives managers a quick snapshot of overall sales activity.
8. List of All Employees
Retrieves basic employee details, sorted alphabetically by last name.
<img width="900" alt="Screenshot 2025-03-13 at 12 32 18 PM" src="https://github.com/user-attachments/assets/731cd665-8777-4b40-ac30-a1f78fe89ddc" />
Provides a quick reference for employee records.
9. Most Used Payment Method
Finds the most frequently used payment methods.
<img width="900" alt="Screenshot 2025-03-13 at 12 32 46 PM" src="https://github.com/user-attachments/assets/e814dd2b-a3da-416e-9576-644b6c67af11" />
Helps managers analyze customer payment preferences.
10. Average TransactionValue
Shows the average transaction value of each customer, meaning the average amount that a customer will spend.
<img width="900" alt="Screenshot 2025-03-13 at 12 33 05 PM" src="https://github.com/user-attachments/assets/b70ac001-0352-436d-95d7-8c7f9afd8c25" />
While this code is quite simple, managers can use this in a variety of ways. Taking a sample set of a few months and using it as a barometer for the following months can allow managers to see if there are fluctuations in the amount that customers usually spend. If significant fluctuations occur during certain parts of the year, managers can conclude that their product/service may have a seasonality component to it. If suddenly consumers start spending less, there may be new competition that has entered the market that the manager may be unaware of. If consumers are buying a lot of product, but there’s a disconnect with the transaction value, the product simply may not be priced high enough
## Database Information:
