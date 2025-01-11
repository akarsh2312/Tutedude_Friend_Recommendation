
# 🚀 Friend Recommendation App

This project is a social networking application that allows users to connect with each other through friend recommendations, friend requests, and search functionalities. The app intelligently suggests friends based on shared interests and mutual friends.

## ✨ Features

- 👤 **User Management**: Users can create accounts, log in, and manage their profile (e.g., avatar, username, interests).
- 🔍 **Search Functionality**: Users can search for other users by name and view their profiles.
- 🤝 **Friend Requests**: Users can send, accept, and reject friend requests.
- 📜 **Friends List**: View and manage your friends, with the option to unfriend.
- 💡 **Friend Recommendations**: The system recommends new friends based on mutual connections and shared interests.

## 🛠 Technologies Used

- **Frontend**: 
  - ⚛️ React
  - 🎨 Tailwind CSS for responsive design
- **Backend**: 
  - 🟢 Node.js 
  - 🛠 Express.js
- **Database**: 
  - 🍃 MongoDB (NoSQL database for storing user and friend data)
- **Authentication**: 
  - 🔐 JWT (JSON Web Tokens for secure authentication)
  
🚀 Installation and Setup

Prerequisites

Node.js

MongoDB

npm or yarn


Steps to Run

1. Clone the repository:

git clone git@github.com:akarsh2312/Tutedude_Friend_Recommendation.git


2. Install dependencies for both frontend and backend:

cd client
npm install
cd ../server
npm install


3. Set up environment variables:

Create a .env file in the root of the server directory and include the following variables:

MONGODB_URI=<Your MongoDB URI>
JWT_SECRET=<Your JWT secret key>

Similary Create a .env file in the root of the client directory and include the following variables:

VITE_API_BASE_URL=<Your backend url>




4. Run the project:

Start the backend server:

cd server
npm start

Start the frontend:

cd client
npm start



5. Open the application in your browser at:

http://localhost:5173



📚 API Endpoints

User Endpoints

POST /api/v1/users/register: Register a new user

POST /api/v1/users/login: Log in an existing user

GET /api/v1/users: Fetch all users


Friend Request Endpoints

POST /api/v1/friend-requests/send/:id: Send a friend request

PUT /api/v1/friend-requests/handle/:id/:id: Accept or reject a friend request

GET /api/v1/friend-requests/received: Get all pending friend requests

GET /api/v1/friend-requests/sent: Get all sent friend requests


Friend Recommendation

GET /api/v1/recommendations: Get friend recommendations based on mutual friends and interests






