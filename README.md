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

## 🧩 Core Modules & API Routes

### 🔐 Authentication
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/login1` | Admin login |
| POST   | `/logout1` | Admin logout |
| POST   | `/register1` | Register new admin |
| POST   | `/register_user` | Register new user |

---

### 👥 Users Management
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_user` | Add new user |
| PUT    | `/update_user/{user}` | Update user info |
| DELETE | `/delete_user/{user}` | Soft delete user |
| GET    | `/trashed_user` | List soft deleted users |
| GET    | `/back_from_soft_delete/{user}` | Restore deleted user |
| GET    | `/get_all_users` | List all users |
| GET    | `/view_user/{userId}` | View user details |

---

### 🧑‍💼 Customers
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_customer` | Add customer |
| PUT    | `/update_customer/{customer}` | Update customer info |
| DELETE | `/delete_customer/{customer}` | Soft delete customer |
| GET    | `/trashed_customer` | View trashed customers |
| GET    | `/back_from_soft_delete/{customer}` | Restore customer |
| GET    | `/get_all_customers` | List all customers |
| GET    | `/get_customer_id/{id}` | Get customer by ID |
| GET    | `/search` | Search customers |

---

### 🗂️ Categories & Departments
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_cat` | Add category |
| DELETE | `/delete_cat/{id}` | Delete category |
| POST   | `/add_department` | Add department |
| GET    | `/get_all_departments` | List all departments |
| GET    | `/get_department_id/{department}` | View department |
| PUT    | `/update_department/{department}` | Update department |
| DELETE | `/delete_department/{department}` | Delete department |

---

### 📦 Products
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_product` | Add product |
| GET    | `/get_all_products` | List all products |
| GET    | `/get_product_id/{id}` | Get product details |
| PUT    | `/update_product/{product}` | Update product |
| DELETE | `/delete_product/{product}` | Delete product |
| POST   | `/add_customer_for_publication` | Associate customer with product publication |

---

### 🧾 Orders
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_order` | Create order |
| GET    | `/get_all_orders` | List all orders |
| DELETE | `/delete_order/{order}` | Delete order |
| GET    | `/ListOrder` | View order list |
| GET    | `/viewOrder` | View order details |
| GET    | `/dd/{orderId}` | Additional order details |

---

### 🚚 Shipments
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_shippment` | Create shipment |
| GET    | `/get_all_shippments` | List shipments |
| PUT    | `/update_Shipement/{shippment}` | Update shipment |
| GET    | `/discounted/{id}` | Apply discount |
| GET    | `/discounted_period_time/{id}` | Discount within period |
| DELETE | `/delete_shippment/{shippment}` | Soft delete shipment |
| GET    | `/trashed_Shipement` | View trashed shipments |
| GET    | `/back_from_soft_delete/{shipment}` | Restore shipment |

---

### 📄 Pages
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_page` | Add sales page |
| GET    | `/get_all_pages` | List pages |
| GET    | `/get_page_id/{id}` | View page details |
| PUT    | `/update_page/{page}` | Update page |
| DELETE | `/delete_page/{page}` | Delete page |
| GET    | `/saled_product/{id}` | Track sold products |
| GET    | `/count_product/{id}` | Count products sold per page |

---

### 🗃️ Records
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_record` | Add record |
| PUT    | `/update_record/{record}` | Update record |
| DELETE | `/delete_recorcd/{record}` | Soft delete record |
| GET    | `/trashed_customer` | View trashed records |
| GET    | `/back_from_soft_delete/{record}` | Restore record |
| GET    | `/get_all_departments` | List department-related records |

---

### ✉️ Invitations
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/add_invtation` | Add invitation |
| GET    | `/get_all_invtations` | List invitations |
| GET    | `/get_invtation/{id}` | View invitation details |
| DELETE | `/delete_invitation/{id}` | Delete invitation |

---

## 🛠️ Tech Stack

- **Backend:** Laravel (PHP)  
- **Database:** MySQL  
- **API Style:** RESTful APIs  
- **Authentication:** Token-based + Middleware  
- **Architecture:** MVC Pattern  
- **Security:** Role-based access control  

---

## ⚙️ Installation

1. Clone the repository:
 ```bash
   git clone https://github.com/Eng-Maya/sales-management-system.git
