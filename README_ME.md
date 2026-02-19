# ShopSmart -- Full Stack E-Commerce Web Application

## Project Overview

ShopSmart is a full-stack E-Commerce web application that allows users
to browse products, add items to cart, place orders, and manage their
accounts securely.

The platform includes an admin dashboard where administrators can manage
products, users, and orders efficiently.

This project demonstrates full-stack development using the MERN stack.

------------------------------------------------------------------------

## Tech Stack

Frontend: - React.js - Axios - React Router - Context API - CSS

Backend: - Node.js - Express.js - MongoDB - Mongoose

Authentication: - JWT (JSON Web Tokens) - bcrypt

Database: - MongoDB

------------------------------------------------------------------------

## Features

### User Features

-   User registration and login
-   JWT-based authentication
-   Browse products
-   View product details
-   Add/remove items from cart
-   Place orders
-   View order history
-   Protected routes

### Admin Features

-   Admin login
-   Add new products
-   Update products
-   Delete products
-   View all orders
-   Manage users

------------------------------------------------------------------------

## Installation

### Prerequisites

-   Node.js installed
-   MongoDB installed and running
-   Git (optional)

------------------------------------------------------------------------

### Backend Setup

cd backend npm install

Create a .env file:

PORT=5000 MONGODB_URI=mongodb://localhost:27017/shopsmart
JWT_SECRET=your_secret_key NODE_ENV=development

Start backend server:

npm start

------------------------------------------------------------------------

### Frontend Setup

cd frontend npm install

Create a .env file:

REACT_APP_API_URL=http://localhost:5000/api

Start frontend:

npm start

Application runs at: http://localhost:3000

------------------------------------------------------------------------

## Project Structure

Backend: backend/ ├── controllers/ ├── models/ ├── routes/ ├──
middleware/ ├── server.js └── package.json

Frontend: frontend/ ├── src/ │ ├── components/ │ ├── pages/ │ ├──
context/ │ ├── App.js │ └── index.js ├── public/ └── package.json

------------------------------------------------------------------------

## API Endpoints

Authentication: - POST /api/auth/register - POST /api/auth/login - GET
/api/auth/verify

Products: - GET /api/products - GET /api/products/:id - POST
/api/products (Admin) - PUT /api/products/:id (Admin) - DELETE
/api/products/:id (Admin)

Cart: - POST /api/cart - GET /api/cart - DELETE /api/cart/:productId

Orders: - POST /api/orders - GET /api/orders/my-orders - GET /api/orders
(Admin)

Users: - GET /api/users (Admin) - DELETE /api/users/:id (Admin)

------------------------------------------------------------------------

## Security Features

-   Password hashing using bcrypt
-   JWT authentication
-   Role-based route protection
-   Environment variables for secrets

------------------------------------------------------------------------

## Future Enhancements

-   Online payment integration (Razorpay / Stripe)
-   Product reviews and ratings
-   Search and filter functionality
-   Image upload with Cloudinary
-   Email order confirmation
-   Cloud deployment

------------------------------------------------------------------------

## License

MIT

------------------------------------------------------------------------

## Support

Feel free to customize and improve this project.
