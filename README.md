# 🧠 ThinkBoard - MERN Stack Notes App

ThinkBoard is a full-stack note-taking application built with the MERN stack (MongoDB, Express, React, Node.js). It allows users to create, read, update and delete notes in a clean and responsive interface.

## 🚀 Features

- 📋 Create and manage notes
- ✏️ Edit and delete notes
- 🧠 Clean and simple UI built with React + Vite
- 🌐 RESTful API built with Express.js
- 💾 MongoDB for persistent data storage
- 🛡️ Rate limiter middleware for backend protection
- 🔧 Environment-based configurations

---

## 🏗️ Project Structure
<pre> /thinkboard 
  ├── /backend # Node.js + Express backend │
     ├── /routes # API route handlers │ 
     ├── /controllers # Request controller logic │ 
     ├── /models # Mongoose schemas │ 
     ├── /config # DB connection and env config │ 
     └── /middleware # Rate limiter, etc. 
  ├── /frontend # React frontend (Vite) │ 
     ├── /src # Source files │ 
     └── /dist # Production build (via vite build) 
  └── README.md # Project documentation </pre>

---

## ⚙️ Tech Stack

- **Frontend**: React, Vite, TailwindCSS (optional)
- **Backend**: Express.js, Node.js
- **Database**: MongoDB with Mongoose
- **Routing**: Express Routers
- **Dev Tools**: Nodemon, dotenv, axios, concurrently
- **Deployment**: Render

---

## 📦 Getting Started

### Prerequisites

- Node.js & npm
- MongoDB Atlas or local MongoDB instance

### 1. Clone the repository

```bash
git clone https://github.com/your-username/thinkboard.git
cd thinkboard
```
### 2. Backend Setup
```bash
cd backend
npm install
```

## Create a .env file:
```bash
MONGO_URI=your_mongodb_uri
PORT=5001
NODE_ENV=development
```

## Run the backend:

```bash
npm run dev
```

### 3. Frontend Setup
```bash
cd ../frontend
npm install
npm run dev
```

The app will run at:

Frontend: http://localhost:5173

Backend: http://localhost:5001/api/notes

## 📡 API Endpoints

|  Method  | Endpoint | Description |
|----------|----------|----------|
| GET  | /api/notes  | Get all notes  |
| GET  | /api/notes/:id  | Get note by ID  |
| POST | /api/notes  | Create a new note  |
| PUT  | /api/notes/:id  | Update an existing note  |
| GET  | /api/notes/:id  | Delete a note  |


## 🛡️ Security Features
- Built-in Rate Limiting middleware to prevent abuse
- Handles CORS for development/production environments

## 📤 Deployment
Frontend (Vercel)
- Link frontend directory to Vercel
- Set build command: npm run build
- Set output directory: dist

Backend (Render/Vercel)
- Point to backend folder
- Set start command: node index.js or use a serverless setup
- Add environment variables

## 🧩 Contributing
Contributions are welcome! Please fork the repo and submit a pull request.

## 📄 License
This project is licensed under the MIT License.

## 🙌 Acknowledgements
Express.js
MongoDB
Vite
React

Built with ❤️ by Mohammed Affaq


