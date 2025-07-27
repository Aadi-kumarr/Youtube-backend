# YouTube Backend Clone

A complete backend system that replicates core functionalities of the YouTube platform. It includes RESTful APIs for user authentication, video management, channel subscriptions, and engagement features.

## Key Features

- User registration and login with JWT-based authentication
- Upload, update, delete, and retrieve videos
- Like/dislike functionality on videos
- Comment system with add/delete features
- Subscribe/unsubscribe to channels
- Video search by title, tags, and other filters
- Fetch trending, random, and user-specific videos

## Tech Stack

- **Node.js** and **Express.js** for backend and routing
- **MongoDB** with **Mongoose** for database management
- **JWT** for authentication and access control
- **Multer** for handling video uploads
- **Bcrypt** for password hashing
- **Postman** for API testing

## Project Structure

- `controllers/` – Handles business logic and DB operations
- `routes/` – Defines API endpoints for users, videos, auth, and comments
- `models/` – MongoDB schemas for Users, Videos, Comments
- `middlewares/` – JWT auth middleware, error handling
- `utils/` – Helper functions and constants

## Setup Instructions

1. Clone the repository
2. Install dependencies: `npm install`
3. Set environment variables in a `.env` file
4. Start the server: `npm start`

## API Documentation

All APIs are tested using Postman. Endpoints include:

- `POST /api/auth/signup`
- `POST /api/auth/login`
- `POST /api/videos/`
- `GET /api/videos/trending`
- `PUT /api/users/subscribe/:channelId`
