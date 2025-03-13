
# MIST 4610 - Project 1 - Group 7:




## Team Name:
- 61608 Group 7
## Team Members:
- Chandler Allmond @chandlerallmond 
- Nick Barton @nicholasbarton1 
- Manav Kamdar 
- Vincent Sengaphone @Sengaphone 
- Landon Wilson @landonnn0 
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
 
 <img width="900" alt="Screenshot 2025-03-13 at 12 28 22 PM" src="https://github.com/user-attachments/assets/9825fb50-3228-4f51-ac76-0a7f42b22c4a" />
  
2. Best Selling Products

<img width="900" alt="Screenshot 2025-03-13 at 12 30 11 PM" src="https://github.com/user-attachments/assets/a70d252a-a1b5-4138-991b-bebf90b33eee" />

  
3. Total Revenue By Product Category

<img width="561" alt="Screenshot 2025-03-13 at 12 30 38 PM" src="https://github.com/user-attachments/assets/d045201d-817f-4fdd-a6b8-92f809db1f5d" />

   
4. Top 3 Most Profitable Brands

<img width="900" alt="Screenshot 2025-03-13 at 12 30 55 PM" src="https://github.com/user-attachments/assets/85e5a732-629e-4bcb-be0c-ebb76f3cb26f" />

   
5. Employee Preformance

<img width="900" alt="Screenshot 2025-03-13 at 12 31 13 PM" src="https://github.com/user-attachments/assets/34a14eab-c2d0-4500-8977-781249cee2f1" />

   
6. Monthly Sales Trends

<img width="900" alt="Screenshot 2025-03-13 at 12 31 41 PM" src="https://github.com/user-attachments/assets/0e9249d5-c9d2-4f36-8515-767167509958" />

    
7. Total Sales Transactions

<img width="900" alt="Screenshot 2025-03-13 at 12 31 59 PM" src="https://github.com/user-attachments/assets/a6e407a2-d051-4a28-8ffc-964a32515420" />

    
8. List of All Employees

<img width="900" alt="Screenshot 2025-03-13 at 12 32 18 PM" src="https://github.com/user-attachments/assets/731cd665-8777-4b40-ac30-a1f78fe89ddc" />

    
9. Most Used Payment Method

<img width="900" alt="Screenshot 2025-03-13 at 12 32 46 PM" src="https://github.com/user-attachments/assets/e814dd2b-a3da-416e-9576-644b6c67af11" />

    
10. Average TransactionValue

<img width="900" alt="Screenshot 2025-03-13 at 12 33 05 PM" src="https://github.com/user-attachments/assets/b70ac001-0352-436d-95d7-8c7f9afd8c25" />

## Database Information:
