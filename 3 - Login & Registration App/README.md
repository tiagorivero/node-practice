# Login & Registration App

An authentication app built with Node.js and Express, practicing user registration, login, and protected routes with JWT.

## Features

- User registration with hashed passwords (bcrypt)
- Login with session handled via a JWT stored in an httpOnly cookie
- Protected route accessible only to logged-in users
- Logout functionality
- Server-rendered views with EJS

## Tech stack

- Node.js
- Express
- EJS
- jsonwebtoken (JWT)
- bcrypt
- db-local (local JSON-based database)

## Backend concepts practiced

- Authentication flow: register, login, logout
- Password hashing and comparison with bcrypt
- Session handling using signed JWTs in httpOnly cookies
- Custom middleware to read and verify the session on every request
- Protected routes based on session state
- Server-side rendering with EJS templates

## Setup

This project needs a secret key to sign JWT tokens.

1. Create a `.env` file in the project root and add:

```
SECRET_JWT_KEY=your_own_random_secret_key
```

You can generate a secure random key by running:

```bash
node -e "console.log(require('crypto').randomBytes(64).toString('hex'))"
```

## Run locally

Clone the repository and install the dependencies:

```bash
npm install
```

Start the server:

```bash
node index.js
```

Open `http://localhost:3000` in your browser.