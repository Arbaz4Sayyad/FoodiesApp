# Foodies - Online Food Ordering System

## Overview
Foodies is a full-stack food ordering application built using the MERN stack (MongoDB, Express.js, React.js, Node.js) and Spring Boot. The app allows users to browse restaurants, place orders, and make secure payments via Razorpay. An admin panel is included for managing orders, users, and restaurants.

## Features
- **User Authentication:** Secure login and signup using JWT authentication.
- **Payment Integration:** Razorpay payment gateway for seamless transactions.
- **AWS S3 Integration:** Stores images securely on AWS S3.
- **Admin Panel:** Manage orders, users, and restaurant details efficiently.
- **Responsive UI:** Developed using React.js with a modern and interactive design.
- **Optimized Backend:** Spring Boot with MongoDB for fast performance and scalability.

## Tech Stack
- **Frontend:** React.js, Redux, Tailwind CSS
- **Backend:** Spring Boot, Node.js, Express.js
- **Database:** MongoDB
- **Cloud Services:** AWS S3
- **Payment Gateway:** Razorpay

## Installation Guide
### 1. Clone the Repository
```sh
git clone https://github.com/your-username/foodies.git
cd foodies
```

### 2. Backend Setup (Spring Boot API)
1. Navigate to the `foodiesapi` folder.
2. Update the `application.properties` file with your credentials:
   ```properties
   spring.data.mongodb.uri = mongodb://localhost:27017/food_delivery_db
   AWS_ACCESS_KEY = your-access-key
   AWS_SECRET_KEY = your-secret-key
   AWS_REGION = your-region
   AWS_BUCKET_NAME = your-bucket-name
   JWT_SECRET = your-secret-key
   RAZORPAY_KEY = your-razorpay-key
   RAZORPAY_SECRET = your-razorpay-secret-key
   ```
3. Start the backend service:
   ```sh
   mvn spring-boot:run
   ```
   The server will start on `http://localhost:8080`.

### 3. Frontend Setup (User Panel)
1. Navigate to the `foodies` folder.
2. Update `constants.js` with your Razorpay key.
3. Install dependencies:
   ```sh
   npm install
   ```
4. Start the frontend:
   ```sh
   npm run dev
   ```
   The user panel will be available at `http://localhost:5174`.

### 4. Admin Panel Setup
1. Navigate to the `adminpanel` folder.
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the admin panel:
   ```sh
   npm run dev
   ```
   The admin panel will be available at `http://localhost:5173`.

## Usage
- Register/Login as a user.
- Browse restaurants and food items.
- Add items to the cart and place an order.
- Make a payment using Razorpay.
- Admins can manage users, orders, and restaurants.

## Contributing
Feel free to fork the repository and submit pull requests!

## Contact
For any issues, reach out to me at **bushansc@gmail.com**

Happy Coding! 🚀
