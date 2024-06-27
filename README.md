# Northwind sample database


## Project Overview
The Northwind database is a sample database created by Microsoft and used for tutorials across various database products for decades. It contains sales data for a fictitious company, “Northwind Traders,” which imports and exports specialty foods globally. This database serves as an excellent tutorial schema for a small-business ERP, encompassing customers, orders, inventory, purchasing, suppliers, shipping, employees, and single-entry accounting. The Northwind database has been ported to numerous non-Microsoft databases, including PostgreSQL.

## Dataset
The dataset used for this analysis is sourced from the YugaByte database and is accessible at the following link: [Northwind Sample Data](https://docs.yugabyte.com/preview/sample-data/northwind/).

## Entity Relationship Diagram (ERD)
![Northwind ERD](https://github.com/DamiData/Northwind-SQL/assets/161587504/3dde62ff-0659-4675-ac6e-ec0e71faff62)


## Data Processing

### Database Table Creation
A database named **Northwind** was created on PostgreSQL to store the dataset. The tables include:

- **Suppliers**: Suppliers and vendors of Northwind
- **Customers**: Customers who buy products from Northwind
- **Employees**: Employee details of Northwind Traders
- **Products**: Product information
- **Shippers**: Details of the shippers who ship products from the traders to the end-customers
- **Orders and Order_Details**: Sales order transactions between the customers and the company

### SQL Scripts
All SQL scripts used for table creation and transformation are provided in the `NorthWIND DATA SET-SQL` directory. These scripts can be executed in a PostgreSQL environment.

## Analysis and Insights
An in-depth analysis of the dataset was conducted to extract meaningful insights to aid decision-making. This involved formulating SQL queries to answer key questions such as:

- Selecting all category names with their descriptions from the category table.
- Listing contact names, customer IDs, and company names of all customers in London.
- Selecting all available columns in the suppliers' table that have fax numbers.
- Listing customer IDs from the orders table with required dates between January 1, 1997, and January 1, 1998, and with freight under 100 units.
- Listing company names and contact names of all owners from customers in Mexico, Sweden, and Germany.
- Counting the number of discontinued products in the products table.
- Listing category names and descriptions of all categories beginning with 'Co'.
- Selecting all company names, cities, countries, and postal codes from the suppliers' table with the word 'rue' in their address, ordered alphabetically by the company name.
- Selecting product IDs and the total quantity for each product in the order details table.
- Selecting customer names and addresses of all customers with orders shipped using Speedy Express.
- Selecting all product names from the product table that are condiments.
- Listing customer names who have no orders in the orders table.
- Adding a shipper name 'Amazon' to the shipper table.
- Changing the company name from 'Amazon' to 'Amazon Prime Shipping' in the shipper table.
- Selecting shipper names and the total freight for each shipper.
- Combining employees' first and last names into a single column aliased as 'Display name'.
- Adding a new customer with an order for 'Grandma's Boysenberry Spread'.
- Listing products along with the total units in stock for each product, with the computed column named 'TotalUnits'.

## Summary and Findings
The project summary and findings are documented in the **NorthWind-SQLProject**. This includes the insights obtained from the data analysis:

- **Categories and Products**: Identified the variety of product categories and their descriptions.
- **Customer Insights**: Analyzed customer distribution, particularly focusing on those in London and specific countries.
- **Supplier and Shipping Analysis**: Examined suppliers with fax numbers and shipments handled by different shippers, particularly 'Speedy Express'.
- **Order Analysis**: Evaluated order details including required dates, freight costs, and products ordered.
- **Product Insights**: Assessed product availability, focusing on discontinued products and stock levels.
- **Employee Information**: Merged employee first and last names for better readability in reports.

These analyses provide a comprehensive understanding of Northwind Traders' operations, helping to inform business decisions related to inventory management, customer relationship management, and supplier coordination.

