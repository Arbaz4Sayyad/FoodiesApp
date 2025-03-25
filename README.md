# Online Food Delivery System

## 📌 Overview
The **Online Food Delivery System** is a full-stack web application that allows users to browse restaurants, order food, make payments, and track deliveries in real-time. It includes an **Admin Panel** for managing orders, users, and menu items.

## 📸 Screenshots

### 🏠 Homepage
![Homepage](food-images/Homepage.png)

### 🛒 Cart
![Cart](food-images/Cart.png)

### 💳 Payment Gateway
![Payment Gateway](food-images/PaymentGateway.png)


## 🚀 Features
- **User Authentication:** JWT-based authentication with role-based access (Admin/User)
- **Restaurant & Menu Management:** Add, update, and remove restaurants and menu items
- **Cart & Order Management:** Users can add food to the cart, place orders, and track their status
- **Payment Integration:** Secure payments using **Razorpay**
- **AWS S3 Integration:** Store and manage images using AWS S3
- **Admin Panel:** Dashboard for managing users, orders, and restaurants
- **Real-time Order Tracking:** Live order updates using WebSockets
- **Responsive UI:** Optimized for desktop & mobile users

---

## 🛠 Tech Stack
### **Frontend:**
- React.js
- Tailwind CSS / Bootstrap
- Redux for state management
- Axios for API requests

### **Backend:**
- Spring Boot (Java) with REST API
- Spring Security (JWT Authentication)
- MongoDB (NoSQL Database)
- Razorpay for Payment Integration
- AWS S3 for storing images
- WebSockets for live tracking

### **DevOps & Tools:**
- Docker & Docker Compose
- Git & GitHub for version control
- Postman for API testing
- VS Code & IntelliJ IDEA

---

## 📂 Project Structure
```plaintext
online-food-delivery-project/
├── foodiesapi/                # Backend (Spring Boot API)
│   ├── src/main/java/com/foodies   # Java Code
│   ├── src/main/resources          # Configuration & Properties
│   ├── pom.xml                     # Maven Dependencies
├── foodies/                   # Frontend (React.js)
│   ├── src/
│   ├── public/
│   ├── package.json
├── adminpanel/                # Admin Dashboard
│   ├── src/
│   ├── package.json
├── README.md
└── .gitignore
```

---

## 🔧 Installation & Setup

### **1️⃣ Clone the Repository**
```sh
git clone https://github.com/Arbaz4Sayyad/MERN_Projects.git
cd online-food-delivery-project
```

### **2️⃣ Backend Setup (Spring Boot - Java)**
```sh
cd foodiesapi
mvn clean install
```
- **Update `application.properties` with your credentials**
- Start the backend server:
```sh
mvn spring-boot:run
```

### **3️⃣ Frontend Setup (React.js)**
```sh
cd ../foodies
npm install
npm run dev
```
- Open browser: **http://localhost:5174**

### **4️⃣ Admin Panel Setup**
```sh
cd ../adminpanel
npm install
npm run dev
```
- Open browser: **http://localhost:5173**

---

## 🔑 Environment Variables
Create a `.env` file in `foodiesapi/src/main/resources/` and add:
```ini
AWS_ACCESS_KEY=your-access-key
AWS_SECRET_KEY=your-secret-key
AWS_REGION=your-region
AWS_BUCKET_NAME=your-bucket-name
JWT_SECRET=your-jwt-secret
RAZORPAY_KEY=your-razorpay-key
RAZORPAY_SECRET=your-razorpay-secret
```

---

## 📡 API Endpoints
| Method | Endpoint | Description |
|--------|---------|-------------|
| POST   | `/api/auth/register` | Register a new user |
| POST   | `/api/auth/login` | User login & token generation |
| GET    | `/api/restaurants` | Get list of restaurants |
| POST   | `/api/orders` | Place a new order |
| GET    | `/api/orders/{id}` | Get order details |
| PUT    | `/api/orders/{id}/status` | Update order status |

---

## 🤝 Contribution Guidelines
We welcome contributions! To contribute:
1. **Fork** the repo & clone locally
2. Create a **new branch** for your feature (`git checkout -b feature-name`)
3. Make changes & commit (`git commit -m "Added new feature"`)
4. Push to GitHub and create a **Pull Request**

---

## 🎯 Future Enhancements
- 📱 Mobile App (React Native)
- 📊 Analytics Dashboard for Admins
- 🌍 Multi-Language Support

---

## 📩 Contact
**Arbaz Sayyad**  
GitHub: [Arbaz4Sayyad](https://github.com/Arbaz4Sayyad)  
Email: arbaz4sayyad@gmail.com  

---

_Enjoy coding & happy development! 🚀_

