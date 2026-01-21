# User Authentication API

A basic user authentication system for secure password hashing.

## Features

- User registration with email/username validation
- Secure password hashing with bcrypt
- User login with credential verification
- MongoDB database integration
- RESTful API endpoints

## Tech Stack

- **Backend:** Express.js
- **Database:** MongoDB 
- **Security:** bcrypt 
- **Environment:** dotenv

## How to Test Endpoints in Postman
Register a User

POST /api/users/register
Content-Type: application/json

{
  "username": "testuser",
  "email": "test@example.com",
  "password": "password123"
}


Login User

POST /api/users/login
Content-Type: application/json

{
  "email": "test@example.com",
  "password": "password123"
}


Test Wrong Login
Just use a wrong password and it should tell you its incorrect in Postman 
