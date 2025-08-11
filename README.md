<h1 align="center">📚 BookWorm – Full‑Stack React Native App 🚀</h1>


##  What we Build


 Works on **real devices & simulators** (Android / iOS)  



---

##  App Features Overview

-  **Auth** — signup & login with JWT, error handling for bad creds
-  **Home Feed** — newest‑first posts with **infinite scrolling**
-  **Create Post** — title, rating, cover image & caption (all required)
-  **Profile Screen** — user info + their posts
-  **Delete Post** — confirmation alert before removal
-  **4 instant themes** — just swap one color object
-  **Web support** — run on `localhost` in the browser
-  **Logout**

---

##  What progress we made 

- Build a REST API with **Node.js**, **Express** & **MongoDB**
-  Implement stateless auth using **JSON Web Tokens (JWT)**
-  Add performant **infinite loading** with pagination cursors
- Handle image uploads the easy way (base64 → Cloudinary)
-  Deploy the backend **for free** (Render / Railway)
-  Ship a cross‑platform app with **React Native + Expo Router**
-  Animate navigation & shared element transitions
- Debug on a physical phone—no Android Studio or Xcode needed

---

##  .env Setup

###  Backend (`/backend`)

```bash
PORT=3000
MONGO_URI=<YOUR_MONGO_DB_URI>
JWT_SECRET=<YOUR_VERY_HARD_TO_FIND_SECRET>

CLOUDINARY_CLOUD_NAME=<YOUR_CLOUDINARY_CLOUD_NAME>
CLOUDINARY_API_KEY=<YOUR_CLOUDINARY_API_KEY>
CLOUDINARY_API_SECRET=<YOUR_CLOUDINARY_API_SECRET>

API_URL=<YOUR_DEPLOYED_API_URL>
```

##  Run the backend

```bash
cd backend
npm install
npm run dev

```

##  Run the mobile

```bash
cd mobile
npm install
npx expo
```


## BookWorm - Full-Stack React Native App
# Project Overview

BookWorm is a complete social book recommendation platform that combines a robust Node.js backend with a modern React Native frontend. It's designed as a mobile-first application where users can share, discover, and manage book recommendations in a social feed format.

## Architecture & Technology Stack
# Backend (Node.js/Express)
Framework: Express.js with ES6 modules
Database: MongoDB with Mongoos
Authentication: JWT (JSON Web Tokens) with bcryptjs password hashing
File Storage: Cloudinary for image uploads (base64 → cloud storage)
Real-time Features: Cron jobs for background tasks
Security: Protected routes with authentication middleware
API Design: RESTful API with pagination support

## Frontend (React Native + Expo)
Framework: React Native with Expo SDK 52
Navigation: Expo Router with typed routes
State Management: Zustand for global state
Storage: AsyncStorage for persistent authentication
UI/UX: Custom styling with theme support
Image Handling: Expo Image Picker with base64 conversion
Cross-Platform: iOS, Android, and Web suppor

## Data Models
1. User Schema
2. Username (unique identifier)
3. Email (unique, for login)
4. Hashed password (bcrypt)
5. Profile image URL
## Timestamps
Book Schema
Title, caption, rating (1-5)
Cloudinary image URL
User reference (ObjectId)
Creation timestamps
## API Endpoints
1. POST /api/auth/register - User registration
2. POST /api/auth/login - User login
3. GET /api/books - Paginated feed
4. POST /api/books - Create recommendation
5. GET /api/books/user - User's posts
6. DELETE /api/books/:id - Delete post

Deployment Ready
1. The application is designed for production deployment with:
2. Environment variable configuration
3. Cloudinary CDN integration
4. MongoDB Atlas compatibility
5. Backend deployment on Render/Railway
6. Mobile app distribution via Expo
## Developer Experience

1. Hot Reload: Both backend (nodemon) and frontend (Expo)
2. Type Safety: TypeScript configuration available
3. Code Quality: ESLint and Prettier setup
4. Testing Ready: Jest configuration included
5. Cross-Platform: Single codebase for iOS, Android, and Web
   
This is a production-ready, full-stack social application that demonstrates modern mobile development practices, secure authentication, cloud storage integration, and scalable architecture patterns. It's perfect for learning full-stack development or as a foundation for a social media application.