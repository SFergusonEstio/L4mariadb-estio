# Tasks to complete:

([Go Back](./README.md))

1. SQL Key Terms
   - Task 1: Create a table to store the details of the following keywords and their definitions, add additional rows as needed.
     
        | **Key Term**        | **Meaning/Definition** |
        |---------------------|------------------------|
        | Data                |                        |
        | Information         |                        |
        | DBMS                |                        |
        | Relational Database |                        |
        | Primary Key         |                        |
        | Foreign Key         |                        |
        | Data Redundancy     |                        |
        | Data Integrity      |                        |
        | DDL                 |                        |
        | DML                 |                        |
        | ...                 |                        |
   - Task 2: Create a table to store the details of different DataTypes and an example of what can be stored within them
     
        | **DataType**         | **Data that can be Stored** |
        |----------------------|-----------------------------|
        | Integer              |                             |
        | Float                |                             |
        | VarChar              |                             |
        | Datatime             |                             |
        | ...                  |                             |
     

#### Before you continue, be sure you have started the database ([Getting Started](./Getting%20Started.md))

2. Creating Databases and Tables
   - Task 1: Create a new database called RelationalTest
   - Task 2: Create the following tables
      - Customer
           - ID
           - FirstName
           - Surname
      - Order
           - ID
           - OrderDate
           - ProductID
           - CustomerID
           - Quantity
           - OrderValue
      - Product
           - ID
           - ProductName
           - Price
   - Task 3: Identify how you would link the above three tables together and set the primary and foreign keys appropriately

([SQL Basics](./sqlbasics.md))

4. SQL Basic Syntax and Key Concepts
   - Task 1: Select all sales from the Sales table
   - Task 2: Display client names with their respective total spent on purchases using a simple join between Clients and Sales tables.

2. Joins and Relationships in SQL
   - Task 3: Show all employees who have not completed any sales yet by performing a left join operation between Employees and Sales table, filtering for NULL values in the SalesID column.
   - Task 4: Create a view that combines client and supplier details to identify high-value clients (based on their total spent) with their corresponding suppliers' information. This will require joining multiple tables using inner joins or left/right outer joins, depending on how you want the data presented.

3. Subqueries and Aggregation
   - Task 5: Find out which client has made the most purchases (i.e., highest total spending) in a given period by calculating aggregates using subqueries or group by statements.
   - Challenge: Write an SQL query to find suppliers who have not provided any stock yet. This requires nested subqueries and joins between Supplier, StockSuppliers, and Product tables.

4. Advanced Joins and Views
   - Task 6: Create a left join view that lists all products in the inventory along with their respective stock levels (quantity) using the Stock table joined with itself through the StockDetails table.
   - Challenge: Write an SQL query to find out which employee has made sales of a product not available in the inventory by joining tables and filtering for NULL values in quantity from the StockDetails table. This involves more complex joins, subqueries or left/right outer joins, and multiple tables being joined together.

5. Optimisation Techniques
   - Task 7: Rewrite an existing query to improve its performance by creating a materialized view of frequently accessed data (for example, the list of clients with high total spending).
   - Challenge: Analyze and optimize a complex SQL query that involves multiple joins, aggregations, subqueries, and/or views. Learners should focus on indexes, execution plans, and query optimization techniques like using EXISTS instead of IN when checking for existence in tables.
