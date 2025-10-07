# 🛒 E-Commerce Application (Django + React)

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-4.x-green?logo=django)](https://www.djangoproject.com/)
[![React](https://img.shields.io/badge/React-18.x-61DAFB?logo=react)](https://react.dev/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Contributions welcome](https://img.shields.io/badge/Contributions-welcome-brightgreen.svg?style=flat)](#-contributing)

A **robust full-stack e-commerce web application** built with **Django (Backend)** and **React (Frontend)**.  
Includes authentication, product management, shopping cart, checkout, and payment integration.

---

## 🚀 Features

### 🧩 Core Functionality

- 🔑 User registration, login, and JWT authentication
- 🛍️ Product listing with search, filter, and category options
- 🧾 Product details with images, descriptions, and reviews
- 🛒 Add to cart, update quantities, and remove items
- 💳 Checkout flow with address, shipping, and payment
- 📦 Order management (for both users & admins)

### 🔐 Admin Dashboard

- Manage products (create, update, delete)
- Manage orders and customers
- View sales analytics (optional add-on)

### 💳 Payment Integration

- Integrated with **Stripe** or **PayPal** for secure payments
- Supports both **test** and **live** payment modes

---

## ⚙️ Tech Stack

| Layer              | Technology                                |
| ------------------ | ----------------------------------------- |
| **Frontend**       | React, Redux Toolkit, Axios, React Router |
| **Backend**        | Django, Django REST Framework             |
| **Database**       | PostgreSQL / SQLite                       |
| **Authentication** | JSON Web Tokens (JWT)                     |
| **Payments**       | Stripe / PayPal                           |
| **Deployment**     | Docker, Nginx, Gunicorn                   |

---

## 🗂️ Project Structure

```bash
ecommerce-app/
├── backend/
│   ├── manage.py
│   ├── core/
│   ├── users/
│   ├── products/
│   ├── orders/
│   ├── payments/
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── vite.config.js or webpack.config.js
│
├── docker-compose.yml
├── README.md
└── .env.example


```
