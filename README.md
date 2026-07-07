# Book Now - Event Booking Platform

A full-stack MERN Event Booking Platform that allows users to browse events, register an account, verify their identity using OTP, and book event tickets online. The application includes secure authentication, booking management, and an admin dashboard for managing events.

## Live Demo

Frontend: https://book-now-iota.vercel.app

Backend API: https://book-now-api-npqr.onrender.com

## GitHub Repository

https://github.com/Anwesha4/book-now

---

## Project Overview

Book Now is a full-stack web application built using the MERN stack. It provides an end-to-end event booking experience with user authentication, event management, and booking functionality. The application follows a client-server architecture with a React frontend, Express backend, and MongoDB database.

---

## Features

### User Features

- User registration
- Secure login using JWT authentication
- Browse available events
- View event details
- Book event tickets
- OTP verification before booking
- Booking confirmation email
- User dashboard

### Admin Features

- Admin authentication
- Create events
- Manage events
- View bookings

---

## Tech Stack

### Frontend

- React.js
- Vite
- React Router
- Axios
- Tailwind CSS

### Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT Authentication
- Nodemailer

### Deployment

- Vercel (Frontend)
- Render (Backend)
- MongoDB Atlas (Database)

---

## Project Structure

```
book-now
│
├── client
│   ├── src
│   ├── public
│   └── package.json
│
├── server
│   ├── controllers
│   ├── middleware
│   ├── models
│   ├── routes
│   ├── utils
│   └── package.json
│
└── README.md
```

---

## Installation

### Clone the Repository

```bash
git clone https://github.com/Anwesha4/book-now.git
```

Move into the project directory.

```bash
cd book-now
```

---

### Backend Setup

```bash
cd server
npm install
```

Create a `.env` file inside the `server` directory.

```env
PORT=5000
MONGODB_URI=your_mongodb_uri
EMAIL_USER=your_email
EMAIL_PASS=your_app_password
JWT_SECRET=your_secret
```

Run the backend server.

```bash
npm run dev
```

---

### Frontend Setup

```bash
cd client
npm install
```

Create a `.env` file.

```env
VITE_API_URL=http://localhost:5000
```

Run the frontend.

```bash
npm run dev
```

---

## API Endpoints

### Authentication

- POST `/api/auth/register`
- POST `/api/auth/login`
- POST `/api/auth/send-otp`
- POST `/api/auth/verify-otp`

### Events

- GET `/api/events`
- GET `/api/events/:id`

### Bookings

- POST `/api/bookings`
- GET `/api/bookings/user`

---

## Authentication

- JWT-based authentication
- Protected routes
- Authorization middleware

---

## Deployment

Frontend deployed on Vercel

Backend deployed on Render

Database hosted on MongoDB Atlas

---

## Known Issues

The deployed application currently experiences occasional OTP email delivery issues due to Gmail SMTP connection timeouts on the hosting platform. Email functionality works correctly in local development. Migrating to a dedicated email service such as Resend is planned.

---

## Future Improvements

- Payment gateway integration
- Search and filter events
- Event categories
- Seat selection
- Email service migration (Resend)
- User profile editing
- Event image uploads
- Pagination

---

## Author

**Anwesha Ganguly**

GitHub: https://github.com/Anwesha4

