# sports-managment
Features
User Authentication: Register and login with JWT-based authentication
Tournament Management: Create and manage tournaments with different sports
Team Registration: Teams can register for tournaments with player details
Match Scheduling: Schedule and track matches with scores and results
Live Leaderboards: Automatic calculation of team standings and points
Admin Panel: Administrative controls for managing the system
Responsive UI: Modern, responsive interface built with React and Tailwind CSS
Tech Stack
Backend
Node.js with Express.js
MongoDB with Mongoose ODM
JWT for authentication
bcryptjs for password hashing
Frontend
React with Vite
Radix UI components
Tailwind CSS for styling
React Query for data fetching
Wouter for routing
Getting Started
Prerequisites
Node.js (v16 or higher)
MongoDB (local or cloud instance)
npm or yarn
Installation
Clone the repository

git clone <repository-url>
cd sports-tournament
Backend Setup

cd backend
npm install
Create a .env file in the backend directory:

PORT=5000
MONGODB_URI=mongodb://localhost:27017/sports-tournament
JWT_SECRET=your-secret-key-here
Start the backend server:

npm run dev
Frontend Setup

cd ../frontend
npm install
npm run dev
Access the Application

Frontend: http://localhost:5173
Backend API: http://localhost:5000
API Endpoints
Authentication
POST /api/auth/register - User registration
POST /api/auth/login - User login
Tournaments
GET /api/tournaments - Get all tournaments
POST /api/tournaments - Create tournament (Admin)
GET /api/tournaments/:id - Get tournament details
Teams
GET /api/teams - Get all teams
POST /api/teams - Register team
GET /api/teams/:id - Get team details
Matches
GET /api/matches - Get all matches
POST /api/matches - Create match (Admin)
PUT /api/matches/:id - Update match result
Leaderboard
GET /api/leaderboard/:tournamentId - Get tournament leaderboard
Project Structure
sports-tournament/
├── backend/
│   ├── config/
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── server.js
│   └── package.json
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── api/
│   │   ├── components/
│   │   ├── contexts/
│   │   ├── hooks/
│   │   ├── lib/
│   │   ├── pages/
│   │   ├── App.jsx
│   │   └── main.jsx
│   ├── index.html
│   ├── package.json
│   └── vite.config.js
├── .gitignore
└── README.md
Contributing
Fork the repository
Create a feature branch
Make your changes
Test thoroughly
Submit a pull request
