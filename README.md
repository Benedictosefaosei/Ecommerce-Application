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

⚙️ Installation & Setup
🔧 Prerequisites

Ensure you have installed:

Python 3.10+

Node.js 18+

PostgreSQL (or use SQLite)

Git

(Optional) Docker

🧱 1. Clone the Repository
git clone https://github.com/yourusername/ecommerce-app.git
cd ecommerce-app

🐍 2. Backend Setup (Django)
cd backend
python3 -m venv venv
source venv/bin/activate # On Windows use venv\Scripts\activate
pip install -r requirements.txt
cp .env.example .env # Update your environment variables
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver

Backend will start at 👉 http://127.0.0.1:8000/

⚛️ 3. Frontend Setup (React)
cd ../frontend
npm install
npm run dev

Frontend will start at 👉 http://localhost:5173/
(or similar port)

🧩 4. Connect Frontend to Backend

In your React .env file:

VITE_API_BASE_URL=http://127.0.0.1:8000/api

🧠 Environment Variables

Create a .env file inside backend/:

DEBUG=True
SECRET_KEY=your-secret-key
DATABASE_URL=postgres://user:password@localhost:5432/ecommerce
STRIPE_SECRET_KEY=your-stripe-secret-key
STRIPE_PUBLIC_KEY=your-stripe-public-key
ALLOWED_HOSTS=localhost,127.0.0.1

🧰 Useful Commands
Command Description
python manage.py runserver Start Django development server
npm run dev Start React development server
python manage.py makemigrations Create new migrations
python manage.py migrate Apply migrations
python manage.py createsuperuser Create admin user
docker-compose up Run full app using Docker
🧪 Testing
🧬 Backend Tests
pytest

🧩 Frontend Tests
npm run test

🚢 Deployment

You can deploy this project using Docker, AWS EC2, Render, or Vercel.

Example (Docker Compose):

docker-compose up --build

📷 Screenshots (optional)
🏠 Home Page 📄 Product Page 💰 Checkout

💡 Future Improvements

✅ Add product recommendations (ML-based)

✅ Implement wishlist & product ratings

✅ Add email notifications

✅ Support multiple vendors

🤝 Contributing

Fork the repository

Create a branch: git checkout -b feature-branch

Commit your changes: git commit -m "Add feature"

Push to branch: git push origin feature-branch

Open a Pull Request

🧑‍💻 Author

Your Name
📧 your.email@example.com

🌐 LinkedIn
• GitHub
