🛒 ShopSmart – Full Stack E-Commerce Web Application
📌 Project Overview

ShopSmart is a full-stack E-Commerce web application built using the MERN stack (MongoDB, Express, React, Node.js).

It allows users to browse products, add items to cart, place orders, and manage their accounts securely.

The application also includes an Admin Dashboard for managing products, users, and orders.

🚀 Tech Stack
🔹 Frontend

React.js

React Router

Axios

Context API

CSS

🔹 Backend

Node.js

Express.js

MongoDB

Mongoose

🔹 Authentication

JWT (JSON Web Token)

bcrypt (Password hashing)

✨ Features
👤 User Features

User Registration & Login

JWT Authentication

Browse Products

View Product Details

Add / Remove Items from Cart

Place Orders

View Order History

Protected Routes

🛠 Admin Features

Admin Login

Add Products

Update Products

Delete Products

View All Orders

Manage Users

🔒 Security Features

Password hashing using bcrypt

JWT-based authentication

Role-based access control

Environment variables for sensitive data

⚙ Installation
📌 Prerequisites

Node.js installed

MongoDB installed and running

🔹 Backend Setup
cd backend
npm install

Create a .env file inside backend folder:

PORT=5000
MONGODB_URI=mongodb://localhost:27017/shopsmart
JWT_SECRET=your_secret_key
NODE_ENV=development

Start backend:

npm start

Backend runs at:
👉 http://localhost:5000

🔹 Frontend Setup
cd frontend
npm install

Create a .env file inside frontend folder:

REACT_APP_API_URL=http://localhost:5000/api

Start frontend:

npm start

Frontend runs at:
👉 http://localhost:3000

📁 Project Structure
Backend
backend/
├── controllers/
├── models/
├── routes/
├── middleware/
├── server.js
└── package.json
Frontend
frontend/
├── src/
│   ├── components/
│   ├── pages/
│   ├── context/
│   ├── App.js
│   └── index.js
├── public/
└── package.json
🔗 API Endpoints
Authentication

POST /api/auth/register

POST /api/auth/login

GET /api/auth/verify

Products

GET /api/products

GET /api/products/:id

POST /api/products (Admin)

PUT /api/products/:id (Admin)

DELETE /api/products/:id (Admin)

Cart

POST /api/cart

GET /api/cart

DELETE /api/cart/:productId

Orders

POST /api/orders

GET /api/orders/my-orders

GET /api/orders (Admin)

📈 Future Enhancements

Online payment integration (Razorpay / Stripe)

Product reviews & ratings

Search & filter functionality

Image upload (Cloudinary)

Email order confirmation

Deployment to cloud

🏆 Project Status

✅ Backend Completed
✅ Frontend Completed
✅ Authentication Implemented
✅ Admin Dashboard Implemented
✅ Documentation Completed

📜 License

MIT
