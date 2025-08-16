🚀 MERN Authentication App

A full-stack authentication system built using MongoDB, Express, React, and Node.js (MERN).
It supports user signup, login, and authentication with secure password hashing and JWT tokens.

✨ Features

🔐 User Signup & Login

🔑 Password hashing with bcrypt

🛡️ JWT authentication for protected routes

☁️ Image upload with Cloudinary (if configured)

⚡ RESTful API (Express + MongoDB)

🎨 React frontend with Axios API calls

📂 Project Structure
project-root/
│── backend/         # Express + MongoDB backend
│   ├── models/      # Mongoose models
│   ├── routes/      # API routes
│   ├── controllers/ # Business logic
│   └── server.js    # Entry point
│
│── frontend/        # React frontend
│   ├── src/
│   ├── public/
│   └── vite.config.js / package.json
│
└── README.md

⚙️ Installation
1️⃣ Clone the Repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

2️⃣ Setup Backend
cd backend
npm install


Create a .env file in backend/:

PORT=5000
MONGO_URI=mongodb://localhost:27017/your-db-name
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret


Run backend:

npm run dev

3️⃣ Setup Frontend
cd ../frontend
npm install
npm run dev

🔌 API Endpoints
Auth Routes
Method	Endpoint	Description
POST	/api/auth/signup	Register new user
POST	/api/auth/login	Login user
GET	/api/auth/me	Get logged-in user
Example Request (Signup)
POST /api/auth/signup
{
  "fullName": "John Doe",
  "email": "john@example.com",
  "password": "123456",
  "bio": "Hello, I'm John!"
}

🖥️ Running the App

Backend runs on: http://localhost:5000

Frontend runs on: http://localhost:5173 (Vite) or 3000 (CRA)

If using proxy in frontend, you can call API with /api/auth/signup directly.
