# Zoom Clone
Zoom Clone is a full-stack video conferencing application built with modern web technologies. It allows users to create or join real-time video meetings, complete with live audio/video, group chat, and screen sharing. The responsive user interface (built with React, Redux, and Tailwind CSS) adapts to different devices and screen sizes. The backend (built with Node.js and Express) handles API requests, authentication, and real-time signaling for meetings.
# Features
1.Video Conferencing: Real-time multi-user video and audio calls, similar to Zoom. Participants can join meetings via unique room URLs.
2.Real-time Chat: In-meeting text chat for participants to communicate during the session.
3.Screen Sharing: Users can share their screen or specific application windows with other participants.
4.Authentication: Secure user authentication and management (e.g., login, registration with JWT or session).
5.Responsive UI: A clean, responsive design using Tailwind CSS that works on both desktop and mobile devices.
6.Easy Meeting Setup: Quickly create a new meeting or join an existing one with minimal steps.
# Tech Stack
The project is split into frontend and backend components, using the following technologies:
Frontend: React.js (UI), Redux (state management), Tailwind CSS (styling), React Router (navigation).
Backend: Node.js, Express.js (REST API and signaling server), Socket.IO (real-time communication), WebRTC (peer-to-peer video/audio streaming).
Database: MongoDB (or another database of your choice) for storing user and meeting data.
Authentication: JWT (JSON Web Tokens) or sessions for secure login.
Development: npm or yarn for package management, ESLint/Prettier for code quality.

# Setup Instructions
Follow these steps to install and run the project locally.

# Prerequisites
Node.js (v14 or higher) and npm (or Yarn) installed.
MongoDB database (local or cloud) if using MongoDB for data persistence.

# Clone Repository
1.Clone the repository: 
git clone https://github.com/Goutam16-Withcode/zoom-clone.git
cd zoom-clone
# Backend Setup
2.Navigate to the backend folder: cd backend
3.Install backend dependencies: npm install
4.Configure environment variables:
Create a .env file inside the backend directory and add the necessary variables, for example: PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
5.Start the backend server: npm start 

# Frontend Setup
6.Open a new terminal and navigate to the frontend folder:cd frontend
7.Install frontend dependencies:npm install
8.Start the frontend development server: npm start

# Folder Structure
An overview of the project directory structure:
zoom-clone/
├── backend/         # Express server (Node.js)
│   ├── controllers/ # Route handlers and business logic
│   ├── models/      # Database schemas/models
│   ├── routes/      # API endpoints
│   ├── utils/       # Utility modules (e.g., middleware, helpers)
│   ├── index.js     # Server entry point
│   └── ...
├── frontend/        # React client application
│   ├── public/      # Static files (HTML, images, etc.)
│   ├── src/         # React source code
│   │   ├── components/ # Reusable UI components
│   │   ├── redux/       # Redux store, actions, reducers
│   │   ├── App.js       # Main app component
│   │   └── ...
│   ├── package.json # Frontend dependencies and scripts
│   └── ...
├── .gitignore       # Ignore list for Git
└── README.md        # Project documentation
The backend folder contains the server code (Express routes, controllers, models, etc.).
The frontend folder contains the React app (components, Redux state management, styles).
