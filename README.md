# Sales Management System 📦

A comprehensive backend API built with **Laravel** to manage sales operations, customers, products, orders, shipments, and administrative workflows.  
This system is designed to support businesses in organizing inventory, handling orders, tracking shipments, and managing users with role-based access.

---

## 🚀 Overview

The Sales Management System provides a structured and scalable RESTful API that enables:

- User and admin authentication
- Product and inventory management
- Customer and order tracking
- Shipment handling
- Department and category organization
- Page-based sales reporting
- Invitation and record management

The project follows clean architecture principles and is suitable for real-world business environments.

---

## 🧩 Core Modules

### 🔐 Authentication & Authorization
- Admin login and logout
- User registration and authentication
- Token-based security
- Middleware protection for admin-only routes

---

### 👥 User Management
- Create and manage users
- Update user information
- Soft delete and restore users
- View active and trashed users

---

### 🧑‍💼 Customer Management
- Add and manage customers
- Update customer profiles
- Soft delete and restore customers
- Search customers

---

### 🗂️ Categories & Departments
- Create and delete categories
- Manage departments
- Assign products to departments
- Update and remove departments

---

### 📦 Product Management
- Add new products
- Update product details
- Delete products
- View product lists and product details
- Associate customers with product publications

---

### 🧾 Orders Management
- Create new orders
- View all orders
- Delete orders

---

### 🚚 Shipment Management
- Create shipments
- Update shipment details
- Track shipment status
- Apply discounts and time-based offers
- Soft delete and restore shipments

---

### 📄 Pages & Sales Tracking
- Create sales pages
- Track sold products
- Count sold products per page
- Update and delete pages

---

### 🗃️ Records Management
- Add operational records
- Update records
- Soft delete and restore records
- View department-related records

---

### ✉️ Invitations
- Send invitations
- View all invitations
- View invitation details
- Delete invitations

---

## 🛠️ Tech Stack

- **Backend:** Laravel (PHP)
- **API Style:** RESTful APIs
- **Authentication:** Token-based + Middleware
- **Database:** MySQL
- **Architecture:** MVC Pattern
- **Security:** Role-based access control

---

## 📂 Project Structure

- Controllers for each module (Users, Products, Orders, Shipments, etc.)
- API routes organized by functionality
- Middleware for admin authorization
- Soft delete support for critical entities

---

## ⚙️ Installation

1. Clone the repository:
 ```bash
   git clone https://github.com/Eng-Maya/sales-management-system.git
```
---
### Install dependencies:
```bash
 composer install
```
---
### Run migrations:
```bash
php artisan migrate
```
---
### Start the server:
```bash
php artisan serve
```
---
