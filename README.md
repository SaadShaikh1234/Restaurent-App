# 🍔 Restaurant Food Ordering WebApp
A modern, full-stack Restaurant Food Ordering Web Application built using the MERN stack (MongoDB, Express.js, React, Node.js). This platform allows users to browse menus, place food orders, manage their carts, and provides an intuitive interface for both customers and potentially restaurant staff.

---

## 🎯 Project Overview
This web application streamlines the food ordering process for restaurants, offering a user-friendly experience for customers to browse dishes, customize orders, and complete purchases. On the backend, it provides a robust API for managing menu items, orders, and user data. It's designed to be scalable and easily customizable for various restaurant needs.

Key aspects of this project include:

• **Customer-facing UI** – Intuitive interface for browsing and ordering.  
• **Shopping Cart Functionality** – Add, remove, and update items before checkout.  
• **Order Management** – Securely process and track orders.  
• **Database Integration** – Store and retrieve menu items, user profiles, and order history.  
• **Authentication (Optional)** – User login/registration for personalized experience.

---

## 🚀 Live Demo / Screenshots
**Live Demo:** 👉 [Click here to try the Restaurant App](https://restaurant-app-mu.vercel.app/)

**Screenshots:**
![1](https://github.com/user-attachments/assets/6ae0c342-cb25-4db6-98d3-1ea8cd9f4acd)![2](https://github.com/user-attachments/assets/9195edd9-5994-441e-b599-3634642d9f37)![3](https://github.com/user-attachments/assets/3e0ace98-9991-4bae-bc77-c831c7e98351)![4](https://github.com/user-attachments/assets/617afec1-4d88-491b-9245-f998be843c17)![5](https://github.com/user-attachments/assets/ff00dfb9-ebe3-493a-b0ab-52ce83a15e2d)![6](https://github.com/user-attachments/assets/917f14d2-a360-45ca-b240-26126d17d273)![7](https://github.com/user-attachments/assets/aae11bd9-a80e-422c-8d5e-a7a3c4ab2348)![8](https://github.com/user-attachments/assets/f3ad626d-1152-4b02-8902-d0a3a6ed5d37)![9](https://github.com/user-attachments/assets/dd7285c4-83a3-4e89-90e8-eca08e32cf4a)![10](https://github.com/user-attachments/assets/8c889edd-509f-45de-86ac-3df228ccaec7)

## ✨ Features
**Customer-Facing:**
• **Browse Menu** – View categories, dishes, descriptions, and prices  
• **Add to Cart** – Easily add/remove items and adjust quantities  
• **Shopping Cart Management** – Review, update, and remove items before checkout  
• **User Authentication** – Register, login, and manage user profiles  
• **Order Placement** – Secure checkout process  
• **Order History** – View past orders  

**Backend/Admin (if applicable):**
• **Menu Management** – Add, update, and delete dishes/categories  
• **Order Tracking** – View and update order statuses  

---

## 💻 Technologies Used
**Frontend:**
• **React.js** – Building the user interface  
• **React Router** – For navigation  
• **Axios / Fetch API** – For making API requests to the backend  
• **Tailwind CSS** – Utility-first CSS framework for fast UI development  
• **Bootstrap** – Responsive layout and component styling

**Backend:**
• **Node.js** – JavaScript runtime environment  
• **Express.js** – Web application framework for the API  
• **MongoDB** – NoSQL database for data storage  
• **Mongoose** – ODM (Object Data Modeling) library for MongoDB

---

## ⚙️ Installation Guide
To get a local copy of the project running on your machine, follow these steps.

**Prerequisites**
• **Node.js** – LTS version recommended  
• **npm** *(or Yarn)* – Node Package Manager for installing dependencies  
• **MongoDB** – Installed locally or access to a MongoDB Atlas cluster

**Backend Setup**
1. Clone the repository:

```Bash

git clone https://github.com/YourGitHubUsername/Restaurant-Food-Ordering-WebApp.git
cd Restaurant-Food-Ordering-WebApp
```
(Replace YourGitHubUsername with your actual GitHub username.)

2. Navigate to the backend directory:

```Bash

cd backend # Or server, api, etc., depending on your folder structure
```

3. Install backend dependencies:

```Bash

npm install
# or yarn install
```

4. Create a .env file:
In the backend directory, create a file named .env and add your MongoDB connection URI and any other environment variables:
```
MONGO_URI=mongodb://localhost:27017/food_ordering_db
PORT=5000
# JWT_SECRET=your_jwt_secret_key (if using authentication)
```
(Adjust MONGO_URI if you are using MongoDB Atlas, and add other variables as needed by your backend.)

**Frontend Setup**
1. Navigate to the frontend directory:

```Bash

cd ../frontend # Or client, webapp, etc.
```

2. Install frontend dependencies:

```Bash

npm install
# or yarn install
```

3. Create a .env file (if needed):
If your frontend needs to know the backend URL, create a .env file in the frontend directory:
```
REACT_APP_BACKEND_URL=http://localhost:5000/api
```
(Adjust the URL to match your backend server.)

---

## ▶️ Usage
**Running the Backend**
1. Start MongoDB: Ensure your MongoDB server is running.
2. Start the backend server: From the backend directory:
```Bash

npm start
# or yarn start
```
The backend API will typically run on http://localhost:5000 (or your specified PORT).

**Running the Frontend**
Start the frontend development server: From the frontend directory:
```Bash

npm start
# or yarn start
```
This command runs the app in development mode. Open http://localhost:3000 to view it in your browser. The page will reload if you make edits.

---

## 📂 Project Structure
Restaurant-App/

├── backend/                  # Node.js/Express.js backend API

│   ├── config/               # Database connection, environment setup

│   ├── models/               # MongoDB schemas (e.g., Dish, User, Order)

│   ├── routes/               # API routes (e.g., dishRoutes.js, userRoutes.js)


│   ├── controllers/          # Business logic for routes

│   ├── middleware/           # Auth middleware, error handling

│   ├── .env.example          # Example environment variables

│   ├── package.json

│   └── server.js             # Main backend server file

├── frontend/                 # React.js frontend application

│   ├── public/

│   ├── src/

│   │   ├── components/       # Reusable UI components (e.g., MenuItem, CartItem)

│   │   ├── pages/            # Main application pages (e.g., HomePage, CartPage, CheckoutPage)

│   │   ├── api/              # API service for frontend-backend communication

│   │   ├── context/          # React Context API for global state (e.g., CartContext, AuthContext)

│   │   ├── assets/           # Images, icons specific to frontend

│   │   ├── App.js

│   │   ├── index.js

│   │   └── index.css

│   ├── .env.example

│   ├── package.json

│   └── README.md             # Frontend-specific README (optional, can be merged)

├── assets/                   # Main project screenshots, GIFs (used in top-level README)

│   ├── restaurant-home.png

│   └── shopping-cart.png

├── .gitignore                # Specifies intentionally untracked files to ignore

└── README.md                 # Project documentation and summary (this file)

---

## 🚧 Future Enhancements
• **Payment Gateway Integration** – Implement secure payment processing (e.g., Stripe, PayPal)  
• **Admin Dashboard** – A dedicated interface for restaurant owners to manage orders, menus, and users  
• **Real-time Updates** – Use WebSockets for live order status updates  
• **User Reviews and Ratings** – Allow customers to review dishes and restaurants  
• **Search and Filters** – Improve menu navigation with robust search and filtering options









