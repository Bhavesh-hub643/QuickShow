# QuickShow 🎬

**Online Movie Ticket Booking System**

QuickShow is a **full-stack web application** developed as a college-level project to understand real-world web development concepts such as authentication, database management, payments, and REST APIs.

The application allows users to browse movies, select seats, and book tickets online, while admins can manage movies and shows.

---

## 📌 Project Objective

The goal of this project is to:

* Learn full-stack development using the MERN stack
* Implement user authentication and authorization
* Handle real-time seat booking logic
* Integrate online payments
* Build an admin panel for management tasks

This project simulates how a real cinema booking system works.

---

## 🛠 Technologies Used

### Frontend

* React.js
* Tailwind CSS
* Vite

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

### Other Tools & Services

* Clerk (authentication)
* Stripe (payment integration)
* Nodemailer (emails)
* Inngest (background jobs)

---

## ✨ Features

### User Features

* User signup and login
* Browse available movies
* View show timings
* Select seats visually
* Book tickets online
* Receive booking confirmation via email

### Seat Booking

* Interactive seat layout
* Real-time seat availability
* Seats are temporarily locked during checkout
* Prevents multiple users from booking the same seat

### Admin Features

* Add and remove movies
* Schedule movie shows
* View all bookings
* Manage platform data

### Payment

* Secure online payments using Stripe
* Payment status verification
* Refund handling for cancelled bookings

---

## 🔐 Authentication

* Users can log in using email or social accounts
* Session management is handled securely
* Supports multiple active sessions

---

## ⚙️ Installation & Setup

### Prerequisites

* Node.js (v16 or above)
* MongoDB (local or Atlas)
* npm

---

### Clone Repository

```bash
git clone https://github.com/Bhavesh-hub643/QuickShow.git
cd QuickShow

```

---

### Backend Setup

```bash
cd backend
npm install
npm run dev
```

---

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🔑 Environment Variables

### Backend `.env`

```env
MONGODB_URI=your_mongodb_uri

CLERK_SECRET_KEY=your_clerk_secret
CLERK_WEBHOOK_SECRET=your_clerk_webhook_secret

STRIPE_SECRET_KEY=your_stripe_secret
STRIPE_WEBHOOK_SECRET=your_stripe_webhook_secret

SMTP_HOST=your_smtp_host
SMTP_PORT=587
SMTP_USER=your_email
SMTP_PASS=your_password

INNGEST_EVENT_KEY=your_inngest_key
INNGEST_SIGNING_KEY=your_inngest_signing_key

PORT=5000
NODE_ENV=development
```

---

### Frontend `.env`

```env
VITE_API_URL=http://localhost:5000
VITE_CLERK_PUBLISHABLE_KEY=your_clerk_key
VITE_STRIPE_PUBLISHABLE_KEY=your_stripe_key
```

---

## 🌐 Application URLs

* Frontend: `http://localhost:3000`
* Backend API: `http://localhost:5000`

---

## 📁 Project Structure

```
quickshow/
├── frontend/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   └── utils/
│
├── backend/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   └── middleware/
│
└── README.md
```

---

## 🔌 API Endpoints (Basic)

### Movies

* GET `/api/movies`
* GET `/api/movies/:id`
* POST `/api/movies` (admin)

### Bookings

* POST `/api/bookings`
* GET `/api/bookings/user/:id`
* PUT `/api/bookings/:id/cancel`

### Payments

* POST `/api/payments/create-intent`
* POST `/api/payments/webhook`

---

## 🧪 Testing

Basic testing can be done by:

* Creating user accounts
* Booking tickets
* Cancelling bookings
* Checking payment and email flow

---

## 🚀 Future Improvements

* Better UI/UX for seat selection
* Search and filter movies
* Mobile responsiveness improvements
* Detailed analytics for admins

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 👨‍🎓 Author

This project was developed as part of academic learning to gain hands-on experience with full-stack web development and real-world application design.


