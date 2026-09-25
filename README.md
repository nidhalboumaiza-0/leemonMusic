# Leemon Music API

A Node.js REST API for a music platform. It organizes songs into albums and categories and includes account-management endpoints for users.

## Features

- User registration and account management
- Song, album, and category resources
- Authentication helpers and email utilities
- MongoDB-backed data models

## Tech Stack

- Node.js and Express
- MongoDB and Mongoose
- JSON Web Tokens
- Nodemailer

## Run Locally

```bash
npm install
npm start
```

Create a local environment file with the database, authentication, and email settings required by the server. Do not commit production credentials.

## Structure

```text
controllers/   Request handlers
models/        Mongoose models
routes/        API routes
utils/         Shared authentication and email helpers
server.js      Application entry point
```
