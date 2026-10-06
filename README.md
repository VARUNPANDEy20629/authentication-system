# 🔐 Full-Stack Authentication System

A secure and responsive **Full-Stack Authentication System** built with **React.js, Node.js, Express.js, and MongoDB**. The application provides user registration, login, JWT-based authentication, protected routes, profile management, and secure password updates.

---

## 🚀 Features

- 🔑 User Registration & Login
- 🔒 JWT-based Authentication
- 🛡️ Protected Routes
- 👤 User Profile Management
- ✏️ Update Personal Information
- 🔐 Secure Password Change
- 🔑 Password Hashing with bcrypt
- 🍃 MongoDB Database Integration
- ⚡ RESTful APIs
- 📡 Axios API Integration
- 🚪 Secure Logout
- 📱 Responsive React Interface

---

## 🛠️ Tech Stack

### Frontend
- React.js
- React Router
- Axios
- HTML5
- CSS3
- JavaScript

### Backend
- Node.js
- Express.js
- JWT
- bcrypt

### Database
- MongoDB
- Mongoose

### Tools
- Git
- GitHub
- VS Code
- npm

---

## 📂 Project Structure

```text
authentication-app/
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   │   ├── Login.jsx
│   │   │   ├── Register.jsx
│   │   │   ├── Dashboard.jsx
│   │   │   └── Profile.jsx
│   │   ├── App.jsx
│   │   └── api.js
│   │
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── models/
│   │   └── User.js
│   ├── routes/
│   │   ├── auth.js
│   │   └── user.js
│   ├── server.js
│   ├── package.json
│   └── ...
│
└── README.md
```

---

## 🔄 Application Flow

```text
        ┌──────────────┐
        │    User      │
        └──────┬───────┘
               │
        ┌──────▼───────┐
        │ Register /   │
        │    Login     │
        └──────┬───────┘
               │
        ┌──────▼───────┐
        │ Express API  │
        └──────┬───────┘
               │
        ┌──────▼───────┐
        │   MongoDB    │
        └──────┬───────┘
               │
        ┌──────▼───────┐
        │ JWT Token    │
        └──────┬───────┘
               │
        ┌──────▼───────┐
        │  Dashboard   │
        │  / Profile   │
        └──────────────┘
```

---

## 🔐 Authentication

The application uses **JSON Web Tokens (JWT)** for authentication.

### Login Process

1. User enters email and password.
2. React sends credentials to the backend.
3. Express validates the credentials.
4. Password is verified using bcrypt.
5. Server generates a JWT token.
6. Token is stored on the client.
7. User is redirected to the dashboard.

### Protected Routes

Protected pages check whether a valid authentication token exists.

```text
No Token
   ↓
Login Page

Valid Token
   ↓
Dashboard
   ↓
Profile
```

---

## 👤 Profile Management

Authenticated users can:

- View their profile
- Update their name
- Update email
- Update phone number
- Update country
- Update address
- Change their password

Password changes require verification of the existing password.

---

## ⚙️ Installation

### 1. Clone the Repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
```

### 2. Navigate to the Project

```bash
cd authentication-app
```

### 3. Install Backend Dependencies

```bash
cd backend
npm install
```

### 4. Install Frontend Dependencies

Open another terminal:

```bash
cd frontend
npm install
```

---

## 🔑 Environment Variables

Create a `.env` file inside the `backend` folder.

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

> ⚠️ Never upload your `.env` file or database credentials to GitHub.

---

## ▶️ Running the Application

### Start Backend

```bash
cd backend
npm start
```

The backend will run on:

```text
http://localhost:5000
```

### Start Frontend

Open another terminal:

```bash
cd frontend
npm start
```

The frontend will run on the development server provided by your React setup.

---

## 🌐 API Endpoints

### Authentication

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login user |
| POST | `/api/auth/logout` | Logout user |

### User

| Method | Endpoint | Description |
|---|---|---|
| GET | `/api/user/profile` | Get user profile |
| PUT | `/api/user/profile` | Update user profile |

---

## 🧠 What I Learned

This project helped demonstrate practical knowledge of:

- React component development
- React Router
- REST API development
- Express.js
- MongoDB & Mongoose
- JWT authentication
- Password hashing with bcrypt
- Protected routes
- Axios
- CRUD operations
- Environment variables
- Full-stack application architecture

---

## 🔮 Future Improvements

- Email verification
- Forgot password functionality
- Google/GitHub OAuth login
- Refresh token implementation
- Role-based authorization
- Admin dashboard
- Two-factor authentication
- Improved UI/UX
- Deployment using cloud platforms

---

## 👨‍💻 Author

**Varun Pandey**

Computer Science Engineering Student  
Interested in **Web Development, AI/ML, and Full-Stack Development**.

---

## ⭐ Support

If you found this project useful, consider giving the repository a ⭐ on GitHub.
