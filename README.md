# 🎟️ Eventora - Full Stack Event Booking Platform

<p align="center">

![React](https://img.shields.io/badge/React-19-blue?logo=react)
![Node.js](https://img.shields.io/badge/Node.js-Express-green?logo=node.js)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-success?logo=mongodb)
![JWT](https://img.shields.io/badge/JWT-Authentication-orange)
![TailwindCSS](https://img.shields.io/badge/TailwindCSS-Styling-38B2AC?logo=tailwind-css)
![License](https://img.shields.io/badge/License-MIT-blue)

</p>

A complete **MERN Stack Event Booking Platform** featuring secure authentication, Email OTP verification, manual payment approval workflow, admin dashboard, event management, booking management, analytics, and responsive UI.

---

# 📸 Project Preview

## Booking System Workflow

<p align="center">
<img src="fc.png" width="900">
</p>

---

## System Sequence Diagram

<p align="center">
<img src="dfd.png" width="900">
</p>

---

# ✨ Features

## 👤 User Features

- Secure Registration
- JWT Authentication
- Password Encryption (bcrypt)
- Email OTP Verification
- Browse Events
- Search Events
- Book Free & Paid Events
- Booking OTP Verification
- Cancel Booking
- Personal Dashboard
- Responsive UI

---

## 👨‍💼 Admin Features

- Secure Admin Login
- Create Events
- Update Events
- Delete Events
- Approve Bookings
- Reject Bookings
- Mark Payment Status
- Revenue Analytics
- Pending Booking Dashboard
- Paid Customer Statistics

---

## 🔐 Security Features

- JWT Authentication
- Protected Routes
- Role Based Authorization
- Password Hashing
- Email OTP Verification
- Booking OTP Verification
- Secure MongoDB Storage

---

# 🛠 Tech Stack

## Frontend

- React.js
- React Router
- Axios
- Tailwind CSS
- React Icons
- Vite

---

## Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcryptjs
- Nodemailer

---

## Database

MongoDB Atlas

---

# 📂 Project Structure

```
EventBooking
│
├── client
│   ├── src
│   │    ├── components
│   │    ├── context
│   │    ├── pages
│   │    ├── utils
│   │    └── App.jsx
│   │
│   └── package.json
│
├── server
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── utils
│   ├── seed.js
│   ├── server.js
│   └── package.json
│
├── assets
│   ├── flowchart.png
│   └── sequence.png
│
└── README.md
```

---

# 🔄 Booking Workflow

### User Registration

```
Register
      ↓
Email OTP
      ↓
Verify OTP
      ↓
Account Activated
```

---

### Booking Flow

```
Select Event
      ↓
Request Booking OTP
      ↓
Receive OTP
      ↓
Verify OTP
      ↓
Booking Created (Pending)
      ↓
Admin Approval
      ↓
Booking Confirmed
      ↓
Confirmation Email
```

---

# ⚙️ Installation Guide

## Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/Event-Booking-System.git

cd Event-Booking-System
```

---

# Backend Setup

```bash
cd server

npm install
```

---

# Frontend Setup

```bash
cd ../client

npm install
```

---

# Environment Variables

Create

```
server/.env
```

Add

```env
PORT=5000

MONGO_URI=your_mongodb_connection_string

JWT_SECRET=your_secret_key

EMAIL_USER=your_email@gmail.com

EMAIL_PASS=your_gmail_app_password
```

---

# Run Backend

```bash
cd server

npm run dev
```

Runs on

```
http://localhost:5000
```

---

# Run Frontend

```bash
cd client

npm run dev
```

Runs on

```
http://localhost:5173
```

---

# Seed Database

Populate MongoDB with demo data.

```bash
cd server

npm run seed
```

Default credentials

### Admin

```
Email

admin@eventora.com

Password

password123
```

---

### User

```
Email

user@eventora.com

Password

password123
```

---

# API Endpoints

## Authentication

```
POST    /api/auth/register

POST    /api/auth/login

POST    /api/auth/verify-otp
```

---

## Events

```
GET     /api/events

GET     /api/events/:id

POST    /api/events

PUT     /api/events/:id

DELETE  /api/events/:id
```

---

## Bookings

```
POST    /api/bookings/send-otp

POST    /api/bookings

GET     /api/bookings/my

PUT     /api/bookings/:id/confirm

DELETE  /api/bookings/:id
```

---

# Authentication Flow

```
User Login
      ↓
JWT Generated
      ↓
Stored in Local Storage
      ↓
Sent in Authorization Header
      ↓
Backend Middleware
      ↓
Protected Routes
```

---

# Email Services

The application automatically sends emails for

- Account Verification OTP
- Booking OTP
- Booking Confirmation

Powered by

- Nodemailer
- Gmail SMTP

---

# Analytics Dashboard

The Admin Dashboard displays

- Total Revenue
- Paid Customers
- Pending Bookings
- Total Events
- Remaining Seats

---

# Future Improvements

- Stripe Payment Gateway
- Razorpay Integration
- QR Ticket Generation
- Event Categories
- Google Login
- Forgot Password
- Event Reviews
- Event Ratings
- Image Upload (Cloudinary)
- PDF Ticket Download
- Admin Charts
- Dashboard Graphs

---

# Author

**Biswajit Sahoo**

GitHub

https://github.com/BiswajitSahoo-Programmer

LinkedIn

https://linkedin.com/in/biswajit-sahoo-1b6940245/

---

# ⭐ Support

If you like this project,

Please consider giving it a ⭐ on GitHub.

It helps the project reach more developers!
