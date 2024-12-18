# Restaurant-Order-Management-Database
A Restaurant Order Management Database project that simulates restaurant operations. It organizes customer, order, menu, reservation, and employee data, ensuring data integrity. The system automates processes like order management and inventory tracking, with realistic data and handling of missing/duplicate values.

## Overview
This repository contains a **Restaurant Order Management Database** project, which simulates a restaurant's operations by managing orders, reservations, customers, menu items, employees, and more. The project uses a structured relational database model with a focus on ensuring data integrity, automating restaurant processes, and providing actionable insights for decision-making.

The system handles different types of data such as nominal, ordinal, interval, and ratio data, reflecting real-world restaurant environments and business operations.

## Features

### **Database Schema**
The database consists of six interconnected tables:
- **Customers**: Stores customer details.
- **Orders**: Tracks orders placed by customers, including status and total amount.
- **Menu Items**: Contains dish categories, prices, and descriptions.
- **Order Details**: Links orders to specific menu items, recording quantities and subtotals.
- **Employees**: Records staff details, positions, and shifts.
- **Reservations**: Manages customer table reservations, including number of guests and reservation dates.

#### **Relationships**
- **Customers** ↔ **Orders**: A customer can place multiple orders.
- **Customers** ↔ **Reservations**: A customer can make multiple reservations.
- **Orders** ↔ **Order Details**: Orders can have multiple menu items, forming a many-to-many relationship.
- **Menu Items** ↔ **Order Details**: A menu item can appear in multiple orders.
- **Employees** ↔ **Orders**: Employees are assigned to manage orders.
  
### **Data**
The database contains randomly generated data:
- 400 customer records
- 600 order records
- 50 menu item records
- 150 reservations
- 25 employee records
- 1500 order detail records

Simulated missing and duplicate values are included in the data to represent real-world scenarios like incomplete orders and repeated information.

### **Design Principles**
- **Normalization**: To reduce redundancy and ensure data integrity.
- **Foreign Keys**: To maintain relationships between tables and enforce referential integrity.
- **Missing & Duplicate Data**: Intentionally added to simulate real-life database challenges and improve data handling.

## Files Included

- **Database File**: `Restaurant_Orders.db` (SQLite Database)
- **Documentation**: `Restaurant Orders DBMS Report.docx`
- **CSV Exports**:
  - `customers.csv`
  - `orders.csv`
  - `menu_items.csv`
  - `order_details.csv`
  - `employees.csv`
  - `reservations.csv`

## Installation and Usage

### Step 1: Clone the Repository
```bash
git clone https://github.com/your-username/restaurant-order-management-database.git
cd restaurant-order-management-database
