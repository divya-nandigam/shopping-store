# API DOCUMENTATION -- ShopSmart

Complete API reference for the ShopSmart E-Commerce system.

**Base URL**: `http://localhost:5000/api`

------------------------------------------------------------------------

## Authentication Endpoints

### 1. User Registration

**Endpoint**: `POST /auth/register`\
**Description**: Register a new user account

``` json
{
  "name": "Divya",
  "email": "divya@example.com",
  "password": "Password123",
  "role": "user"
}
```

------------------------------------------------------------------------

### 2. User Login

**Endpoint**: `POST /auth/login`\
**Description**: Login user and receive JWT token

``` json
{
  "email": "divya@example.com",
  "password": "Password123"
}
```

------------------------------------------------------------------------

### 3. Verify Token

**Endpoint**: `GET /auth/verify`\
**Headers**: `Authorization: Bearer token`

------------------------------------------------------------------------

## Product Endpoints

### 4. Get All Products

**Endpoint**: `GET /products`

### 5. Get Product by ID

**Endpoint**: `GET /products/:id`

### 6. Add Product (Admin Only)

**Endpoint**: `POST /products`

### 7. Update Product (Admin Only)

**Endpoint**: `PUT /products/:id`

### 8. Delete Product (Admin Only)

**Endpoint**: `DELETE /products/:id`

------------------------------------------------------------------------

## Cart Endpoints

### 9. Add to Cart

**Endpoint**: `POST /cart`

### 10. Get User Cart

**Endpoint**: `GET /cart`

### 11. Remove Item from Cart

**Endpoint**: `DELETE /cart/:productId`

------------------------------------------------------------------------

## Order Endpoints

### 12. Create Order

**Endpoint**: `POST /orders`

### 13. Get User Orders

**Endpoint**: `GET /orders/my-orders`

### 14. Get All Orders (Admin Only)

**Endpoint**: `GET /orders`

------------------------------------------------------------------------

## Admin Endpoints

### 15. Get All Users

**Endpoint**: `GET /users`

### 16. Delete User

**Endpoint**: `DELETE /users/:id`

------------------------------------------------------------------------

## Error Responses

### 400 -- Bad Request

``` json
{
  "message": "Validation error"
}
```

### 401 -- Unauthorized

``` json
{
  "message": "Invalid or missing token"
}
```

### 403 -- Forbidden

``` json
{
  "message": "Access denied"
}
```

### 404 -- Not Found

``` json
{
  "message": "Resource not found"
}
```

### 500 -- Server Error

``` json
{
  "message": "Internal server error"
}
```

------------------------------------------------------------------------

## Version Information

-   API Version: 1.0\
-   Backend: Node.js + Express.js\
-   Database: MongoDB\
-   Authentication: JWT
