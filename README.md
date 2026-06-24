# MERN Bookstore — BookVerse

A full-featured e-commerce bookstore application built with the MERN stack (MongoDB, Express, React, Node.js), featuring Redux state management, JWT authentication, a mock payment flow, and a robust Admin control panel.

## Prerequisites
- Node.js (v14 or higher)
- npm or yarn
- MongoDB (local community edition)

## Setup & Installation

### Step 1: Start Local MongoDB
Make sure MongoDB is running on your machine:
```bash
# On Windows, you can start the MongoDB service from Services.msc, or run in cmd/PowerShell:
net start MongoDB
# Or run mongod directly if it is added to your PATH:
mongod
```

### Step 2: Seed the Database
Once MongoDB is running, navigate to the `server/` directory and seed the catalog:
```bash
cd server
node seed.js
```
This sets up standard genres, featured books, and test accounts:
- **Admin Login**: `admin@bookstore.com` / `adminpassword`
- **Regular Customer Login**: `john@gmail.com` / `password123`

### Step 3: Run the Application
From the root directory (`d:\Mern`), run the following command to start both the Express API server (port 5000) and the React frontend development server (port 3000):
```bash
npm run dev
```

Visit `http://localhost:3000` to browse, purchase, and test.

---

## Folder Structure & Key Features
- **Server**: Configured with strict schemas, Express routes protected by JWT + Admin middleware, and error-handling filters.
- **Client**: Implemented using Redux Toolkit for cart and session sync.
- **Theme**: Premium dark glassmorphism styling utilizing Outfit typography, dynamic borders, and slide-in notifications.
