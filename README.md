Grocery Ordering System - REST API

Problem Statement

Develop a RESTful API service using Spring Boot to manage an online grocery ordering system. The system supports CRUD operations for customers, grocery items, and orders, focusing on basic data management without complex business logic.

Requirements

This is a simplified online grocery system aimed at maintaining records of customers, grocery items, and orders.

Entities

Customer: Stores customer information.

Grocery Item: Represents the available grocery items.

Order: Tracks orders placed by customers for grocery items.

Relationships

A customer can place multiple orders.

An order can contain one or more grocery items.

A grocery item can be part of multiple orders.

CRUD Operations

Customer Management

Fields: Name, Email, Address, Phone

Perform CRUD operations to manage customer information.

Grocery Item Management

Fields: Name, Category, Price, Quantity

CRUD operations to manage grocery items.

Order Management

Fields: Customer, Grocery Item(s), Order Date, Total Price

CRUD operations to manage order details.

REST API Endpoints

Customer Endpoints

GET /customers - Retrieve all customers

GET /customers/{id} - Retrieve a specific customer

POST /customers - Create a new customer

PUT /customers/{id} - Update an existing customer

DELETE /customers/{id} - Delete a customer

Grocery Item Endpoints

GET /grocery-items - Retrieve all grocery items

GET /grocery-items/{id} - Retrieve a specific grocery item

POST /grocery-items - Add a new grocery item

PUT /grocery-items/{id} - Update an existing grocery item

DELETE /grocery-items/{id} - Remove a grocery item

Order Endpoints

GET /orders - Retrieve all orders

GET /orders/{id} - Retrieve a specific order

POST /orders - Create a new order

PUT /orders/{id} - Update an existing order

DELETE /orders/{id} - Delete an order

Technologies Used

Java

Spring Boot

Spring Data JPA

H2 Database (for in-memory storage)

RESTful API Design

Maven/Gradle

How to Run the Project

Clone the repository:

git clone https://github.com/mandarpatil0331/grocery-app.git

Navigate to the project directory:

cd grocery-app

Build and run the application:

mvn spring-boot:run

The API will be available at http://localhost:8080

Future Enhancements

Implement user authentication and authorization.

Add payment integration for orders.

Improve search and filtering for grocery items.

Integrate external databases such as MySQL or PostgreSQL.
