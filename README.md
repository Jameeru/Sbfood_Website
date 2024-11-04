Food Ordering Website

This project is a food ordering website built using the MEAN stack (MongoDB, Express.js, Angular, and Node.js). The application allows users to browse food items, add them to their cart, and place orders seamlessly.

Table of Contents

Features
Technologies Used
Getting Started
Installation
Usage
API Endpoints
Contributing
License
Features

User registration and authentication
Browse and search food menu
Add items to the shopping cart
Place and view orders
User profile management
Technologies Used

Frontend: Angular, Bootstrap
Backend: Node.js, Express.js
Database: MongoDB
Authentication: JWT (JSON Web Tokens)
Getting Started

Prerequisites
Node.js (v14 or higher)
MongoDB (locally installed or use MongoDB Atlas)
Angular CLI (install via npm)
Installation
Clone the repository:
bash
Copy code
git clone https://github.com/yourusername/food-ordering-website.git
cd food-ordering-website
Install dependencies for the backend:
bash
Copy code
cd server
npm install
Install dependencies for the frontend:
bash
Copy code
cd ../client
npm install
Create a .env file in the backend directory and add your MongoDB connection string:
makefile
Copy code
MONGODB_URI=mongodb://<username>:<password>@localhost:27017/foodOrdering
JWT_SECRET=your_jwt_secret
Usage

Running the Application
Start the backend server:
bash
Copy code
cd server
npm start
Start the Angular frontend:
bash
Copy code
cd client
ng serve
Open your browser and navigate to http://localhost:3000.
API Endpoints

User Routes
POST /api/users/register - Register a new user
POST /api/users/login - Login a user
GET /api/users/profile - Get user profile (protected)
Food Routes
GET /api/food - Get all food items
POST /api/food - Add a new food item (admin only)
PUT /api/food/:id - Update a food item (admin only)
DELETE /api/food/:id - Delete a food item (admin only)
Order Routes
POST /api/orders - Create a new order
GET /api/orders/user/:id - Get orders for a specific user
Contributing

Contributions are welcome! Please fork the repository and submit a pull request.

License

This project is licensed under the MIT License. See the LICENSE file for details.
