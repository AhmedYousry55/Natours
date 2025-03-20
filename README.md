# Natours Application

Built using modern technologies: node.js, express, mongoDB, mongoose .

# 🌍 Natours - A Tour Booking API  

## 📌 Overview  

Natours is a **RESTful API** for a tour booking application, built with **Node.js**, **Express.js**, and **MongoDB**. This project is designed to handle user authentication, manage tour packages, process payments, and support advanced filtering, pagination, and sorting functionalities.  

The backend follows best practices in API development, including data validation, security implementation, and error handling.  

## 🚀 Features  

✅ **User Authentication & Authorization** (JWT-based)  
✅ **CRUD Operations** for Tours, Users, and Reviews  
✅ **Advanced Filtering, Sorting & Pagination**  
✅ **Image Upload & Processing** (Multer & Sharp)  
✅ **Stripe Payment Integration**  
✅ **Data Security & Rate Limiting**  
✅ **Geospatial Queries for Nearby Tours**  
✅ **Automated Email Notifications**  

## 🛠️ Tech Stack  

- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (Mongoose ODM)  
- **Authentication:** JWT, bcrypt  
- **Payment Gateway:** Stripe  
- **Cloud Storage:** Cloudinary (Optional)  
- **Email Service:** Nodemailer  
- **Middleware & Security:** Helmet, CORS, Rate Limiting  

## 📂 Project Structure  

Natours/
│── controllers/      # Route handlers (Business logic)
│── models/           # Mongoose models
│── routes/           # Express routes
│── public/           # Static assets
│── utils/            # Helper functions
│── config.env        # Environment variables
│── server.js         # Entry point
│── package.json      # Dependencies
│── README.md         # Project documentation


## 🏗️ Installation & Setup  

1. **Clone the repository**  
   ```sh
   git clone https://github.com/AhmedYousry55/Natours.git
   cd Natours
2. **Install dependencies**
   npm install
3. **Set up environment variables**
   Create a .env file in the root directory and add:
   PORT=3000
   DATABASE=your_mongodb_connection_string
   JWT_SECRET=your_secret_key
   STRIPE_SECRET_KEY=your_stripe_key
   EMAIL_USERNAME=your_email
   EMAIL_PASSWORD=your_password
4. **Run the development Server**
   npm run dev
5. **Access the API**
   The server runs on http://localhost:3000/api/v1/

## 🔗 API Endpoints
### Authentication
**POST /api/v1/users/signup - Register a new user**

**POST /api/v1/users/login - Log in**

**GET /api/v1/users/logout - Log out**

**POST /api/v1/users/forgotPassword - Reset password**

## Tours
**GET /api/v1/tours - Get all tours**

**GET /api/v1/tours/:id - Get a single tour**

**POST /api/v1/tours - Create a new tour (Admin only)**

**PATCH /api/v1/tours/:id - Update tour (Admin only)**

**DELETE /api/v1/tours/:id - Delete tour (Admin only)**

## Bookings
**POST /api/v1/bookings/checkout-session/:tourId - Stripe checkout**

**GET /api/v1/bookings - Get all bookings**

**For the complete list of endpoints, check the routes/ directory.**

## 🛡️ Security & Best Practices
**JWT-based authentication to secure user data**

**Rate limiting & CORS to prevent API abuse**

**Sanitization & validation to prevent NoSQL injection and XSS attacks**

**Secure password hashing using bcryptjs**



