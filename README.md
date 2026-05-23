# QuickBlog

A full-stack blogging platform with a public blog listing, admin dashboard, AI-enhanced content generation, and image upload optimization.

---

## 🌟 Features

- Public blog listing and individual blog detail pages
- Admin panel for adding, deleting, and toggling publish status
- Rich-text blog editor using Quill
- AI-powered summary generation and optional content generation
- Image uploads with ImageKit optimization
- Comment submission and moderation support
- Category filtering and search for blogs
- Responsive UI with dark mode support

---

## 🧩 Project Structure

- `client/` — React front-end built with Vite and TailwindCSS
- `server/` — Express backend with MongoDB and Gemini AI integration

---

## ⚙️ Tech Stack

### Frontend
- React 19
- Vite
- TailwindCSS
- React Router DOM
- Axios
- Quill
- Moment.js
- React Hot Toast

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- ImageKit
- Google Gemini AI
- JWT-based auth for admin actions

---

## 🚀 Setup

### Backend

1. Navigate to the server folder:
   ```bash
   cd server
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file with the following values:
   ```env
   PORT=3000
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   GEMINI_API_KEY=your_gemini_api_key
   IMAGEKIT_PUBLIC_KEY=your_imagekit_public_key
   IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
   IMAGEKIT_URL_ENDPOINT=your_imagekit_url_endpoint
   ```
4. Start the backend:
   ```bash
   npm run server
   ```

### Frontend

1. Open a second terminal and navigate to the client folder:
   ```bash
   cd client
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` or `.env.local` file with the API base URL:
   ```env
   VITE_BASE_URL=http://localhost:3000
   ```
4. Run the client:
   ```bash
   npm run dev
   ```

---

## 📝 Notes

- Public blog endpoints are served from the backend at `/api/blog`.
- Admin routes require authentication and use a JWT token header.
- Unpublished blogs are hidden from public access.

---

## 📌 Usage

- Visit the client app in the browser to view blogs.
- Access the admin area via `/admin` and log in to manage posts.
- Use the admin panel to create, publish/unpublish, and delete blogs.

