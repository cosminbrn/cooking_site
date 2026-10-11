# Cooking Site

A full-stack recipe-sharing app where users can sign up, publish recipes with photos, and rate and review each other's dishes.

<!-- Add 2–3 screenshots or a GIF here, e.g. ![Home](docs/home.png) -->

## Features

- **Accounts**: registration and login with bcrypt-hashed passwords and JWT sessions
- **Recipe upload**: publish a recipe with title, description and image
- **Browse and search** recipes, plus a top-rated section on the home page
- **Ratings and reviews** that update the average rating and review count instantly, with no page refresh
- **Profile page** showing the signed-in user's details

## Stack

| Layer    | Tech                                              |
| -------- | ------------------------------------------------- |
| Frontend | React 18, React Router 7, Vite                    |
| Backend  | Node.js, Express, Mongoose, Multer (image uploads) |
| Database | MongoDB                                           |
| Auth     | JSON Web Tokens, bcryptjs                         |

## Running locally

Requires Node.js 18+ and a MongoDB database

```bash
# Backend (http://localhost:3000)
cd backend
cp .env.example .env   # then fill in MONGODB_URI and JWT_SECRET
npm install
npm run dev

# Frontend (http://localhost:5000), in a second terminal
cd frontend
npm install
npm run dev
```

## Project structure

```
backend/    Express API, Mongoose models, image uploads
frontend/   React app (Vite)
```
