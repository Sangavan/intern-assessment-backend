# Intern Assessment - Backend

A RESTful API built with NestJS, MongoDB, and JWT authentication.

## Tech Stack
- NestJS
- MongoDB (Mongoose)
- JWT Authentication (HTTP-only cookies)
- Bcrypt password hashing
- Class Validator

## Live URL
https://intern-assessment-backend.onrender.com

## Setup Instructions

### 1. Clone the repo
```bash
git clone https://github.com/Sangavan/intern-assessment-backend.git
cd intern-assessment-backend
```

### 2. Install dependencies
```bash
npm install
```

### 3. Create `.env` file (use `.env.example` as reference)
```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=3000
NODE_ENV=development
FRONTEND_URL=http://localhost:3001
```

### 4. Run the app
```bash
npm run start:dev
```

## API Endpoints

### Auth
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /auth/register | Register a new user |
| POST | /auth/login | Login and get JWT cookie |
| POST | /auth/logout | Logout and clear cookie |

### Users (Protected)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /users | Get all users |
| GET | /users/:id | Get single user |
| PUT | /users/:id | Update user |
| DELETE | /users/:id | Delete user |