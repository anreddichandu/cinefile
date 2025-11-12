# cinefile

# 🚀 PROJECT IDEA: Cinefile - A Movie Trailer & Buzz Management App

Build a **Full Stack MERN (MongoDB, Express, React, Node.js)** application named **Cinefile**.  
I, as an **admin**, should be able to **manually add new movies and buzz/news updates**, and the frontend should automatically display them for all users.

## 🌟 FEATURES

### 🎬 MOVIES MODULE
- Admin can:
  - Add new movie: title, poster URL, YouTube trailer link, description, release date, genre
  - Edit or delete any movie
- Users can:
  - See all added movies
  - Click "Watch Trailer" to open the trailer link
  - View description, genre, release date

### 📰 BUZZ MODULE
- Admin can:
  - Add new buzz/news post: headline, content, image URL
  - Edit or delete buzz posts
- Users can:
  - Read all latest buzz updates in the frontend

### 👤 ADMIN AUTHENTICATION
- Login system (JWT + bcrypt)
- Only logged-in admin can access dashboard (Add/Edit/Delete forms)

### 🧩 BACKEND REQUIREMENTS
- Use **Node.js + Express**
- Connect to **MongoDB Atlas**
- Create models:
  - `Movie` (title, posterUrl, trailerUrl, description, releaseDate, genre, createdAt)
  - `Buzz` (headline, content, imageUrl, createdAt)
  - `User` (username, password) for admin auth
- Routes:
  - `/api/movies` → CRUD operations for movies
  - `/api/buzz` → CRUD operations for buzz
  - `/api/auth` → login/signup for admin
- Use `dotenv` for environment variables and `cors` for frontend connection.

### 🎨 FRONTEND REQUIREMENTS
- Use **React.js (Vite or CRA)** + **Tailwind CSS** for UI
- Pages:
  - Home (lists latest movies)
  - Buzz (shows news updates)
  - Admin Login
  - Admin Dashboard (AddMovieForm + AddBuzzForm)
- Components:
  - MovieCard
  - BuzzCard
  - AddMovieForm
  - AddBuzzForm
  - Navbar
  - Footer
- Fetch data from backend using REST APIs.
- Use React Router for navigation.
- When admin adds a new movie or buzz → it should instantly appear in the frontend.

### ⚙️ PROJECT STRUCTURE
Cinefile/
 ├── client/ (React frontend)
 │   ├── src/
 │   │   ├── components/
 │   │   ├── pages/
 │   │   ├── context/
 │   │   ├── App.jsx
 │   │   └── index.js
 │   └── package.json
 └── server/ (Node backend)
     ├── models/
     ├── routes/
     ├── controllers/
     ├── server.js
     └── package.json

### 🌍 DEPLOYMENT
- Frontend → Vercel
- Backend → Render or Railway
- Database → MongoDB Atlas

### 🧾 README.md CONTENT
- Project description
- Features list
- Tech stack used
- Steps to run locally
- Deployment links (Frontend, Backend)
- Screenshots (optional)

# ⚡ GOAL
Generate all necessary boilerplate code, models, routes, and React components for this “Cinefile” project.
It should be production-ready, clean, and beginner-friendly.

