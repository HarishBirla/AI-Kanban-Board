<div align="center">

# 🤖 AI Kanban Board

### 🚀 AI-Powered Real-Time Project Management Platform

An intelligent Kanban board that combines **real-time collaboration**, **AI-powered productivity**, and a **modern responsive interface** to help teams plan, organize, and complete projects efficiently.

<p align="center">

<img src="https://img.shields.io/badge/React-19-61DAFB?style=for-the-badge&logo=react&logoColor=white"/>
<img src="https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white"/>
<img src="https://img.shields.io/badge/Express-black?style=for-the-badge&logo=express"/>
<img src="https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white"/>

</p>

<p align="center">

<img src="https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socketdotio"/>
<img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"/>
<img src="https://img.shields.io/badge/JWT-black?style=for-the-badge&logo=jsonwebtokens"/>
<img src="https://img.shields.io/badge/Google_Gemini-4285F4?style=for-the-badge&logo=google&logoColor=white"/>
<img src="https://img.shields.io/badge/Neon_Database-00E699?style=for-the-badge"/>

</p>

<p align="center">

<img src="https://img.shields.io/github/license/HarishBirla/AI-Kanban-Board?style=flat-square"/>
<img src="https://img.shields.io/github/stars/HarishBirla/AI-Kanban-Board?style=flat-square"/>
<img src="https://img.shields.io/github/forks/HarishBirla/AI-Kanban-Board?style=flat-square"/>
<img src="https://img.shields.io/github/issues/HarishBirla/AI-Kanban-Board?style=flat-square"/>

</p>

</div>

---

# 📖 Overview

Managing projects efficiently requires much more than a traditional task board.

**AI Kanban Board** is a modern full-stack project management platform that combines the flexibility of Kanban workflows with AI-powered assistance and real-time collaboration.

It enables teams to organize work visually, collaborate instantly, automate repetitive planning tasks using Google Gemini AI, and monitor project progress through analytics.

The application follows a scalable client-server architecture with secure JWT authentication, PostgreSQL database, Socket.IO powered synchronization, and a responsive UI built using React and Tailwind CSS.

---

# ✨ Key Features

| Feature | Description |
|----------|-------------|
| 🔐 Authentication | Secure Login & Registration using JWT + bcrypt |
| 📋 Boards Management | Create, rename, recolor and delete project boards |
| 📂 Shared Boards | Invite teammates and collaborate together |
| 👥 Team Roles | Owner, Admin and Member permissions |
| 📌 Drag & Drop | Smooth Kanban workflow using dnd-kit |
| 📝 Tasks | Complete CRUD operations with rich task details |
| 📅 Due Dates | Schedule and organize deadlines |
| 📊 Dashboard Analytics | Workload insights and project statistics |
| ⚡ Real-Time Collaboration | Live synchronization using Socket.IO |
| 🤖 AI Backlog Generation | Generate complete project backlogs using Gemini |
| 🧠 AI Task Breakdown | Convert large goals into actionable subtasks |
| 📄 AI Sprint Summary | AI generated sprint progress summaries |
| 🔍 Search & Filtering | Quickly locate boards and tasks |
| 📱 Fully Responsive | Optimized for Desktop, Tablet and Mobile |
| 🎨 Modern UI | Premium interface built with Tailwind CSS |

---

# 🚀 Why This Project?

Unlike traditional Kanban boards, this application integrates **Artificial Intelligence** directly into the project management workflow.

Instead of manually planning every task, users can simply describe their project idea and allow AI to:

- Generate complete task backlogs
- Break complex features into smaller subtasks
- Summarize sprint progress
- Improve team productivity
- Accelerate project planning

Combined with real-time collaboration, this creates a highly efficient development workflow.

---

# 🛠️ Tech Stack

| Layer | Technology |
|--------|------------|
| Frontend | React 19, Vite |
| Styling | Tailwind CSS v4 |
| Backend | Node.js, Express.js |
| Database | PostgreSQL (Neon) |
| Authentication | JWT, bcrypt |
| AI Engine | Google Gemini API |
| Real-Time | Socket.IO |
| State Management | React Context API |
| HTTP Client | Axios |
| Drag & Drop | dnd-kit |
| Animations | Framer Motion |

---

# 🧰 Core Technologies

### Frontend

- React 19
- Vite
- React Router
- Tailwind CSS
- Axios
- Socket.IO Client
- Context API
- Framer Motion
- dnd-kit

### Backend

- Node.js
- Express.js
- PostgreSQL
- JWT Authentication
- bcrypt
- Socket.IO
- dotenv
- CORS

### AI

- Google Gemini API

### Database

- PostgreSQL
- Neon Cloud Database

---

# 🌟 Highlights

✅ AI-powered project planning

✅ Real-time collaboration

✅ Multi-board management

✅ Role-based authorization

✅ Secure authentication

✅ Modern responsive interface

✅ Clean MVC architecture

✅ RESTful APIs

✅ PostgreSQL database

✅ Socket.IO synchronization

✅ Gemini AI integration

---

# 📷 Application Preview

> Add screenshots here after deployment.

| Login | Dashboard |
|-------|-----------|
| ![](screenshots/login.png) | ![](screenshots/dashboard.png) |

| Kanban Board | Analytics |
|-------------|-----------|
| ![](screenshots/board.png) | ![](screenshots/analytics.png) |

--- 

# 🏗️ Project Architecture

```
                        ┌──────────────────────────┐
                        │      React + Vite        │
                        │    Tailwind CSS v4 UI    │
                        └─────────────┬────────────┘
                                      │
                              REST APIs + Socket.IO
                                      │
                     ┌────────────────┴────────────────┐
                     │                                 │
             Express.js Backend                Socket.IO Server
                     │                                 │
        JWT Authentication & APIs          Live Collaboration
                     │
          PostgreSQL Database (Neon)
                     │
            Google Gemini AI Integration
```

---

# 📂 Project Structure

```text
AI-Kanban-Board
│
├── backend
│   ├── src
│   │   ├── config
│   │   ├── controllers
│   │   ├── db
│   │   ├── middleware
│   │   ├── realtime
│   │   ├── routes
│   │   ├── services
│   │   ├── socket
│   │   ├── utils
│   │   └── index.js
│   │
│   ├── package.json
│   ├── package-lock.json
│   └── .env
│
├── frontend
│   ├── public
│   ├── src
│   │   ├── assets
│   │   ├── components
│   │   ├── context
│   │   ├── hooks
│   │   ├── lib
│   │   ├── pages
│   │   ├── routes
│   │   ├── App.jsx
│   │   └── main.jsx
│   │
│   ├── package.json
│   ├── vite.config.js
│   └── .env
│
├── README.md
└── .gitignore
```

---

# ⚙️ Getting Started

## Clone Repository

```bash
git clone https://github.com/HarishBirla/AI-Kanban-Board.git

cd AI-Kanban-Board
```

---

# 📦 Install Dependencies

## Backend

```bash
cd backend

npm install
```

## Frontend

```bash
cd frontend

npm install
```

---

# 🔐 Environment Variables

## Backend (.env)

```env
PORT=5050

NODE_ENV=development

CLIENT_URL=http://localhost:5173

DATABASE_URL=YOUR_NEON_DATABASE_URL

JWT_SECRET=YOUR_SECRET_KEY

JWT_EXPIRES_IN=7d

GEMINI_API_KEY=YOUR_GEMINI_API_KEY

GEMINI_MODEL=gemini-2.5-flash
```

---

## Frontend (.env)

```env
VITE_API_URL=http://localhost:5050

VITE_SOCKET_URL=http://localhost:5050
```

---

# 🗄️ Database Setup

This project uses **PostgreSQL** hosted on **Neon Database**.

### Create a Neon Database

1. Create a Neon account.
2. Create a PostgreSQL database.
3. Copy the database connection string.
4. Paste it into

```env
DATABASE_URL=
```

inside

```
backend/.env
```

---

# ▶️ Run Backend

```bash
cd backend

npm run dev
```

Server starts at

```
http://localhost:5050
```

---

# ▶️ Run Frontend

```bash
cd frontend

npm run dev
```

Application starts at

```
http://localhost:5173
```

---

# 📜 Available Scripts

## Backend

```bash
npm run dev
```

Runs backend using Nodemon.

```bash
npm start
```

Runs production server.

---

## Frontend

```bash
npm run dev
```

Starts Vite development server.

```bash
npm run build
```

Creates production build.

```bash
npm run preview
```

Preview production build locally.

---

# 🔑 Authentication Flow

```
User Login/Register
        │
        ▼
Express API
        │
        ▼
Password Hashing (bcrypt)
        │
        ▼
JWT Generated
        │
        ▼
Token Stored on Client
        │
        ▼
Protected API Requests
```

---

# ⚡ Real-Time Workflow

```
User moves card
       │
       ▼
Socket.IO Event
       │
       ▼
Backend validates request
       │
       ▼
Database Updated
       │
       ▼
Broadcast to connected users
       │
       ▼
Everyone sees changes instantly
```

---

# 🤖 AI Features

Powered by **Google Gemini API**

### AI Backlog Generation

Describe a project idea and receive:

- Epics
- User stories
- Tasks
- Priorities

---

### AI Task Breakdown

Convert a large feature into:

- Smaller tasks
- Actionable subtasks
- Better sprint planning

---

### AI Sprint Summary

AI analyzes board activity and generates:

- Sprint progress
- Remaining work
- Productivity insights
- Team summary

---

# 🔒 Security

- JWT Authentication
- Password hashing with bcrypt
- Protected Routes
- Environment Variables
- PostgreSQL Parameterized Queries
- Role Based Authorization
- Socket Authentication

---

# 📡 REST API Modules

```
Authentication

Boards

Columns

Tasks

Users

AI

Real-time Events
```

---

# 📡 API Overview

## Authentication

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login user |
| GET | `/api/auth/me` | Get logged-in user |

---

## Boards

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/boards` | Get all boards |
| POST | `/api/boards` | Create board |
| GET | `/api/boards/:id` | Get board details |
| PATCH | `/api/boards/:id` | Update board |
| DELETE | `/api/boards/:id` | Delete board |

---

## Columns

| Method | Endpoint |
|--------|----------|
| POST | `/api/columns` |
| PATCH | `/api/columns/:id` |
| DELETE | `/api/columns/:id` |

---

## Tasks

| Method | Endpoint |
|--------|----------|
| POST | `/api/tasks` |
| GET | `/api/tasks/:id` |
| PATCH | `/api/tasks/:id` |
| DELETE | `/api/tasks/:id` |

---

## AI

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/ai/backlog` | Generate AI backlog |
| POST | `/api/ai/breakdown` | Break task into subtasks |
| POST | `/api/ai/summary` | Generate sprint summary |

---

# 🎨 UI Highlights

- 🎯 Modern Dashboard
- 📊 Analytics Cards
- 📅 Calendar View
- 📋 Kanban Interface
- 🌙 Dark Theme
- 💫 Smooth Animations
- 🎨 Beautiful Tailwind UI
- 📱 Fully Responsive Design
- ⚡ Fast Loading Experience

---

# 🚀 Deployment

The application can be deployed using the following platforms.

## Frontend

- Vercel
- Netlify

## Backend

- Render
- Railway

## Database

- Neon PostgreSQL

---

# 📈 Future Improvements

- 📌 Email Notifications
- 📌 Google Authentication
- 📌 GitHub Authentication
- 📌 File Attachments
- 📌 Comments & Mentions
- 📌 Activity Timeline
- 📌 Team Chat
- 📌 Time Tracking
- 📌 Sprint Planning
- 📌 Workspace Templates
- 📌 AI Meeting Notes
- 📌 AI Burndown Reports
- 📌 Mobile Application

---

# ⚙️ Performance Optimizations

- Lazy Loading
- Component Reusability
- Optimized API Calls
- Socket Event Optimization
- PostgreSQL Transactions
- Modular Architecture
- Clean MVC Pattern
- Protected Routes
- Responsive UI
- Efficient State Management

---

# 🏆 Project Highlights

✔ Full Stack Application

✔ RESTful API

✔ Real-Time Collaboration

✔ AI Powered Productivity

✔ JWT Authentication

✔ PostgreSQL Database

✔ Socket.IO Integration

✔ Responsive UI

✔ Modern Architecture

✔ Cloud Database

✔ Clean Code Structure

✔ Production Ready Design

---

# 🤝 Contributing

Contributions are welcome!

1. Fork the repository

2. Create a new branch

```bash
git checkout -b feature/awesome-feature
```

3. Commit your changes

```bash
git commit -m "Add awesome feature"
```

4. Push to your branch

```bash
git push origin feature/awesome-feature
```

5. Open a Pull Request

---

# 📝 License

This project is licensed under the **MIT License**.

See the **LICENSE** file for more information.

---

# 👨‍💻 Author

## Harish Birla

Computer Science Engineering Student

Full Stack MERN Developer

AI & Backend Enthusiast

GitHub:

```
https://github.com/HarishBirla
```

LinkedIn:

```
https://www.linkedin.com/in/your-linkedin/
```

---

# 🙏 Acknowledgements

Special thanks to the amazing open-source community.

- React
- Vite
- Express.js
- PostgreSQL
- Neon
- Socket.IO
- Tailwind CSS
- Google Gemini
- dnd-kit
- Framer Motion

---

# ⭐ Show Your Support

If you found this project helpful,

⭐ Star this repository

🍴 Fork it

🛠️ Contribute

📢 Share it

---

<div align="center">

## ⭐ If you like this project, don't forget to star the repository!

Made with ❤️ by **Harish Birla**

</div>
