# TaskFlow — Full Stack Task Manager

A full-stack task management web app built with Node.js, Express, MongoDB, and vanilla JavaScript.

## 🔗 Live Demo
[TaskFlow Live](https://vanshpatawari0605.github.io/TaskFlow/)

## 🛠️ Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js + Express.js
- **Database:** MongoDB + Mongoose
- **Auth:** JWT (JSON Web Tokens) + bcryptjs
- **Deploy:** GitHub Pages (frontend) + Render (backend) + MongoDB Atlas (database)

## ✨ Features
- User registration & login with JWT authentication
- Create, read, update, delete tasks (full CRUD)
- Filter tasks by status (pending / in-progress / completed)
- Filter tasks by priority (high / medium / low)
- Real-time stats dashboard showing total, pending, in-progress and completed tasks
- Fully responsive design

## 🚀 Getting Started

### Prerequisites
- Node.js installed
- MongoDB installed locally

### Installation
1. Clone the repo
2. Install backend dependencies
3. Start the backend server
4. Open `index.html` in your browser

## 📁 Project Structure
TaskFlow/
├── index.html
├── backend/
│   ├── server.js
│   └── package.json
└── README.md

## 🔌 API Endpoints

| Method | Endpoint | Description | Auth |
|--------|----------|-------------|------|
| POST | /api/auth/register | Register user | No |
| POST | /api/auth/login | Login user | No |
| GET | /api/tasks | Get all tasks | Yes |
| POST | /api/tasks | Create task | Yes |
| PUT | /api/tasks/:id | Update task | Yes |
| DELETE | /api/tasks/:id | Delete task | Yes |

## 🔐 How Auth Works
- User registers/logs in → server returns a JWT token
- Token is stored in localStorage
- Every API request sends the token in the Authorization header
- Server verifies the token using middleware before allowing access

## 👨‍💻 Author
**Vansh Patawari**
- Email: vanshpatawari@gmail.com
- GitHub: [VanshPatawari0605](https://github.com/VanshPatawari0605)
- LinkedIn: [Vansh Patawari](https://linkedin.com/in/vanshpatawari)

## 📄 License
MIT
