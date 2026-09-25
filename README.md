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

1. Install Node.js 18 or newer and start MongoDB locally, or prepare a MongoDB Atlas connection.
2. Open a terminal in the repository root and install dependencies:

   ```bash
   npm install
   ```

3. The server loads `config.env`, so create or update that file with development values:

   ```dotenv
   NODE_ENV=development
   PORT=3000
   DATABASE=mongodb://127.0.0.1:27017/leemon_music
   JWT_SECRET=replace-with-a-long-random-value
   JWT_EXPIRE_IN=1d
   EmailMailer=your-development-email
   EmailPassword=your-email-app-password
   ```

4. Start the API:

   ```bash
   npm start
   ```

5. Keep the terminal open and call the API through `http://localhost:3000` unless `PORT` was changed.

Do not commit real database, authentication, or email credentials.

## Structure

```text
controllers/   Request handlers
models/        Mongoose models
routes/        API routes
utils/         Shared authentication and email helpers
server.js      Application entry point
```
