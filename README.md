# OMNITAAS - Login Application

A modern full-stack login application built with React and Node.js/Express.

## Project Structure

```
OMNITAAS_project/
├── client/              # React frontend (Vite)
│   ├── src/
│   │   ├── App.jsx      # Main app component with routing
│   │   ├── Login.jsx    # Login form component
│   │   ├── Welcome.jsx  # Welcome page component
│   │   ├── App.css      # Styling for all components
│   │   └── main.jsx     # React entry point
│   ├── package.json
│   └── vite.config.js
└── server/              # Node.js/Express backend
    ├── server.js        # Main server file
    └── package.json
```

## Features

- ✨ Modern, responsive UI with gradient design
- 🔐 User authentication system
- 🚀 Full-stack application (React + Express)
- 💾 Persistent login state using localStorage
- 🎯 Clean and organized code structure

## Prerequisites

- Node.js (v14 or higher)
- npm (comes with Node.js)

## Installation

### Setup Server

```bash
cd server
npm install
```

### Setup Client

```bash
cd client
npm install
```

## Running the Application

### Start the Backend Server

From the `server` directory:

```bash
npm start
```

The server will run on `http://localhost:5000`

### Start the Frontend Development Server

From the `client` directory:

```bash
npm run dev
```

The client will run on `http://localhost:5173`

## Login Credentials

- **Username:** `admin`
- **Password:** `admin`

## Technologies Used

### Frontend
- React 19
- React Router DOM
- Vite (build tool)
- CSS3 (modern styling)

### Backend
- Node.js
- Express.js
- CORS (for cross-origin requests)

## Features Overview

### Login Page
- Username and password input fields
- Client-side validation
- Error message display
- Username persistence in localStorage

### Welcome Page
- Personalized greeting
- Logout functionality
- Session management

## API Endpoints

### POST /login
Authenticates user credentials

**Request Body:**
```json
{
  "username": "admin",
  "password": "admin"
}
```

**Success Response (200):**
```json
{
  "message": "Login successful"
}
```

**Error Response (401):**
```json
{
  "message": "Invalid credentials"
}
```

## Available Scripts

### Client Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build
- `npm run lint` - Run ESLint

### Server Scripts
- `npm start` - Start the server

## Future Enhancements

- Add user registration page
- Integrate with a database (MongoDB, PostgreSQL)
- Implement password hashing and JWT tokens
- Add more user roles and permissions
- Email verification system

## License

MIT
