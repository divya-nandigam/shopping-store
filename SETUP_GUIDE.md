# INSTALLATION AND SETUP GUIDE

## Complete Installation Guide for ShopSmart -- E-Commerce Application

Follow these step-by-step instructions to set up and run the ShopSmart
application on your local machine.

------------------------------------------------------------------------

## STEP 1: Prerequisites

1.  Node.js and npm\
    Download: https://nodejs.org/\
    Verify: node --version\
    npm --version

2.  MongoDB\
    Download: https://www.mongodb.com/try/download/community\
    Start MongoDB service before running the project.

3.  Code Editor (VS Code recommended)

------------------------------------------------------------------------

## STEP 2: Project Setup

Navigate to your project folder:

cd
"c:`\Users`{=tex}`\YourName`{=tex}`\Downloads`{=tex}`\ShopSmart`{=tex}"

Project structure:

ShopSmart/ ├── backend/ ├── frontend/ ├── README.md └── .gitignore

------------------------------------------------------------------------

## STEP 3: Backend Setup

### Install Dependencies

cd backend\
npm install

### Create .env File

PORT=5000\
MONGODB_URI=mongodb://localhost:27017/shopsmart\
JWT_SECRET=your_super_secret_key\
NODE_ENV=development

### Start Backend Server

npm start

Expected Output: Server running on port 5000\
MongoDB connected successfully

Backend URL: http://localhost:5000

------------------------------------------------------------------------

## STEP 4: Frontend Setup

Open new terminal:

cd frontend\
npm install

Create .env file:

REACT_APP_API_URL=http://localhost:5000/api

Start frontend:

npm start

Application URL: http://localhost:3000

------------------------------------------------------------------------

## STEP 5: Testing

1.  Register new user\
2.  Login\
3.  Browse products\
4.  Add to cart\
5.  Place order\
6.  Login as admin\
7.  Add / Update / Delete products\
8.  View all orders

------------------------------------------------------------------------

## STEP 6: Database Verification

Open MongoDB shell:

mongosh

Inside shell:

show databases\
use shopsmart\
show collections

Expected collections: - users\
- products\
- orders\
- carts

------------------------------------------------------------------------

## STEP 7: Production Build

Build frontend:

cd frontend\
npm run build

Production .env example:

NODE_ENV=production\
MONGODB_URI=mongodb+srv://username:password@cluster.mongodb.net/shopsmart\
JWT_SECRET=strong_production_secret

Deploy backend and frontend to your preferred cloud platform.

------------------------------------------------------------------------

## Troubleshooting

Port 5000 in use: netstat -ano \| findstr :5000

MongoDB connection failed: Ensure MongoDB is running and MONGODB_URI is
correct.

Module not found: Delete node_modules and run npm install again.

------------------------------------------------------------------------

## Features Checklist

-   User Registration & Login\
-   Product Management\
-   Cart Functionality\
-   Order Management\
-   Admin Dashboard\
-   JWT Authentication\
-   Role-based Access

------------------------------------------------------------------------

Congratulations!\
ShopSmart is successfully set up and ready to use.
