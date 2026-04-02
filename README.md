# Order Management Application

---

## Overview
The **Order Management Application** is a Java-based system designed to handle clients, products, orders, and invoices. The application allows users to add, modify, delete, and view data, while automatically updating stock and generating invoices.  

---

## Objectives
The main goal of this project is to simulate an order management system for a small business. Secondary objectives include:  
- Efficiently manage clients, products, and orders.  
- Automatically generate bills when orders are placed.  
- Ensure intuitive and user-friendly interfaces.  

---

## Requirements

### Functional Requirements
- Add, update, delete, and view clients.  
- Add, update, delete, and view products.  
- Add, delete, and view orders.  
- Generate and view invoices for completed orders.  

### Non-Functional Requirements
- The application must be intuitive and easy to use.  
- Ensure data integrity and validation for all input fields.  

---

## Architecture
The application is divided into five main packages:

1. **BusinessLogic**  
   - Handles business rules and validations (e.g., `ClientBLL`, `ProductBLL`, `OrderBLL`, `BillBLL`).  
   - Validators: `EmailValidator`, `QuantityValidator`.  

2. **Connection**  
   - Manages database connections via `ConnectionFactory`.  

3. **DataAccess**  
   - Provides DAO classes for database interactions: `ClientDAO`, `ProductDAO`, `OrderDAO`, `BillDAO`.  

4. **Model**  
   - Contains data models: `Client`, `Product`, `Order`, `Bill`.  

5. **Presentation**  
   - GUI classes: `ClientView`, `ProductView`, `OrderView`, `BillView`, `View`, `Controller`.  

---

## Features
- **Graphical User Interface (GUI):** Switch between Client, Product, Order, and Bill interfaces.  
- **CRUD Operations:** Create, read, update, delete for clients, products, and orders.  
- **Data Validation:** Email format validation, stock quantity checks.  
- **Invoice Generation:** Automatically generates bills upon successful order placement.  
- **Reflection-Based Table Display:** Dynamically displays database records in tables.  

---

## Installation
1. Clone the repository:  
```bash
git clone <repository-url>
