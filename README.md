# online-course-platform
A full-stack MERN application for managing online courses

# Online Course Management Platform – MERN Stack

A modern full-stack web application built with the MERN (MongoDB, Express.js, React.js, Node.js) stack for managing online courses. The platform allows users to register, authenticate, and perform full CRUD operations on their own courses through a secure and user-friendly interface.

---

## Features

- ✅ Secure registration and login with JWT authentication
- ✅ Full CRUD for courses (Create, Read, Update, Delete)
- ✅ Real-time updates using Redux Toolkit + RTK Query
- ✅ Protected routes with backend middleware
- ✅ State management with Redux Toolkit
- ✅ Responsive frontend built with React and React Router

---

## Technologies Used

**Frontend:**
- React.js
- Redux Toolkit & RTK Query
- React Router
- Tailwind CSS (optional if used)

**Backend:**
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT (jsonwebtoken)
- Bcrypt.js

---

## Authentication Flow

1. User submits login form (email & password)
2. Request is sent to `/api/auth/login`
3. The backend verifies credentials and returns a JWT token
4. Token is stored in localStorage and used in future API requests
5. Protected routes on the backend verify the token via middleware

---

# 1. Clone the repository
git clone https://github.com/yourusername/online-course-platform.git
cd online-course-platform

# 2. Backend setup
cd server
npm install
# Add your .env file here with MONGO_URI and JWT_SECRET
node index.js

# 3. Frontend setup
cd ../client
npm install
npm start


MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
