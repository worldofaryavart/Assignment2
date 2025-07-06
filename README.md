 # Simple E-commerce API

This project is a simple e-commerce backend API built with Node.js, Express, and MongoDB. It supports user authentication (JWT), role-based access (customer/admin), product management, cart, and order creation.

## Features
- User registration and login (JWT authentication)
- Customer and admin roles
- Product listing, search, pagination
- Cart management (add, update, remove items)
- Order creation from cart
- Admin product management (add, update, delete)
- Basic HTML frontend (placeholder)

## Getting Started
1. Clone the repo or download the code.
2. Run `npm install` to install dependencies.
3. Set up your `.env` file (see `.env` for example).
4. Start MongoDB locally or use MongoDB Atlas.
5. Run `npm run dev` to start the server with nodemon.
6. Use Postman or the provided HTML page to test endpoints.

## API Endpoints
- `POST /api/auth/register` — Register a new user
- `POST /api/auth/login` — Login and get JWT
- `GET /api/products` — List products (with pagination/search)
- `POST /api/products` — Add product (admin only)
- `PUT /api/products/:id` — Update product (admin only)
- `DELETE /api/products/:id` — Delete product (admin only)
- `GET /api/cart` — Get current user's cart
- `POST /api/cart/add` — Add item to cart
- `PUT /api/cart/update` — Update cart item
- `DELETE /api/cart/remove/:productId` — Remove item from cart
- `POST /api/orders` — Create order from cart
- `GET /api/orders` — Get user's orders

## User Roles
- **Customer:** Can view products, manage cart, and place orders.
- **Admin:** Can also manage products.

## License
MIT
