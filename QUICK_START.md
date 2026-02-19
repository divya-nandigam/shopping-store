# QUICK START GUIDE

Get ShopSmart -- E-Commerce Application up and running in 5 minutes!

------------------------------------------------------------------------

## Prerequisites Checklist

-   Node.js installed (https://nodejs.org/)
-   MongoDB installed and running
-   Code editor (VS Code recommended)

------------------------------------------------------------------------

## Quick Setup (Windows)

### 1. Open PowerShell and Navigate to Project

cd
"c:`\Users`{=tex}`\YourName`{=tex}`\Downloads`{=tex}`\ShopSmart`{=tex}"

### 2. Start Backend (Terminal 1)

cd backend npm install npm start

Wait for: Server running on port 5000

### 3. Start Frontend (Terminal 2)

cd frontend npm install npm start

Application opens at: http://localhost:3000

------------------------------------------------------------------------

## Quick Setup (Mac/Linux)

### 1. Navigate to Project

cd \~/path/to/ShopSmart

### 2. Start Backend (Terminal 1)

cd backend npm install npm start

### 3. Start Frontend (Terminal 2)

cd frontend npm install npm start

------------------------------------------------------------------------

## First Login

### Create User Account:

1.  Click Register
2.  Enter:
    -   Name: Divya
    -   Email: divya@example.com
    -   Password: Test@123
3.  Click Sign Up

------------------------------------------------------------------------

## Key Features to Test

### As User:

-   Browse products
-   Add to cart
-   Remove from cart
-   Place order
-   View order history

### As Admin:

-   Add product
-   Update product
-   Delete product
-   View orders
-   Manage users

------------------------------------------------------------------------

## .env Files

### Backend .env

PORT=5000 MONGODB_URI=mongodb://localhost:27017/shopsmart
JWT_SECRET=your_secret_key NODE_ENV=development

### Frontend .env

REACT_APP_API_URL=http://localhost:5000/api

------------------------------------------------------------------------

## Useful Commands

Backend: npm start npm run dev

Frontend: npm start npm run build

MongoDB: mongosh show databases use shopsmart show collections

------------------------------------------------------------------------

## API Base URL

http://localhost:5000/api

------------------------------------------------------------------------

You're all set! Happy coding!
