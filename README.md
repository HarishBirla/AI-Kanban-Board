<div align="center">

# 🚀 AI Kanban Board

### A real-time, AI-powered project management board built on the PERN stack

*Describe a goal in one line — Google Gemini turns it into a fully prioritized backlog.*
*Your whole team drags, drops, and collaborates live — instantly, over Socket.IO.*

<br/>

[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![React](https://img.shields.io/badge/React_19-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://react.dev/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)

[![Socket.IO](https://img.shields.io/badge/Socket.IO-010101?style=for-the-badge&logo=socket.io&logoColor=white)](https://socket.io/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS_v4-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Google Gemini](https://img.shields.io/badge/Google_Gemini-8E75B2?style=for-the-badge&logo=googlegemini&logoColor=white)](https://ai.google.dev/)
[![JWT](https://img.shields.io/badge/JWT-Auth-black?style=for-the-badge&logo=jsonwebtokens&logoColor=white)](https://jwt.io/)

<br/>

[![Framer Motion](https://img.shields.io/badge/Framer_Motion-black?style=flat-square&logo=framer&logoColor=blue)](https://www.framer.com/motion/)
[![dnd-kit](https://img.shields.io/badge/dnd--kit-Drag_&_Drop-orange?style=flat-square)](https://dndkit.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](LICENSE)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

</div>

---

## ✨ Overview

**AI Kanban Board** is a full-stack project management tool where an entire team can plan, organize, and track
work together in real time — with **Google Gemini AI** doing the heavy lifting of turning ideas into an
actionable, prioritized backlog.

Type a one-line goal like *"Launch our v2 mobile app"* and watch AI generate a complete backlog of
prioritized tasks. Break any big task into clean subtasks with one click. Get an instant AI-written summary of
your sprint — what's done, what's at risk, and what needs focus — all without leaving the board.

---

## 🎯 Key Features

| | Feature | Description |
|---|---|---|
| 🔐 | **Authentication** | Secure register/login with JWT + bcrypt, protected routes, auto-login on refresh |
| 📋 | **Boards Management** | Create, recolor, rename & delete boards — "My Boards" and "Shared with You" views |
| 🖱️ | **Drag & Drop Kanban** | Smooth card movement across columns powered by `@dnd-kit`, fully persisted to Postgres |
| 📊 | **Columns** | Add, rename, reorder, and delete columns with position-based ordering |
| ✅ | **Tasks (Full CRUD)** | Title, description, priority, due date, assignee — all in a rich task modal |
| 👥 | **Board Sharing & Roles** | Invite teammates, assign owner/admin/member roles, share/unshare instantly |
| ⚡ | **Real-Time Collaboration** | Every move, edit, and add syncs instantly via Socket.IO, with live presence avatars |
| 🤖 | **AI Backlog Generation** | Describe a goal → Gemini returns a full, prioritized task backlog |
| 🧩 | **AI Task Breakdown** | Turn any big task into clear, actionable subtasks with one click |
| 📈 | **AI Sprint Summary** | Gemini reads your board and summarizes progress in plain English |
| 📉 | **Dashboard Analytics** | KPI cards, board workload analytics, and a live recent-activity feed |
| 🗂️ | **My Tasks, Calendar & Team** | Cross-board task list, due-date calendar, and a full team directory |
| 🏢 | **Multi-Tenant Ready** | Every board, column, and task is member-scoped — users see only what they're part of |
| 🧱 | **Clean Architecture** | Routes → Controllers → Services, raw SQL with `pg`, JWT middleware, transactional seeding |
| 🎨 | **Premium Responsive UI** | Tailwind v4 theme tokens, Framer Motion animations, hand-built shadcn-style components |

---

## 🛠️ Tech Stack

<div align="center">

| Layer | Technology |
|---|---|
| **Database** | PostgreSQL (raw SQL via `pg`, no ORM) |
| **Backend** | Node.js, Express.js |
| **Real-Time** | Socket.IO |
| **Auth** | JWT, bcrypt |
| **AI Engine** | Google Gemini API |
| **Frontend** | React 19, Vite |
| **Styling** | Tailwind CSS v4 + hand-built shadcn-style UI kit |
| **Drag & Drop** | `@dnd-kit/core`, `@dnd-kit/sortable` |
| **Animation** | Framer Motion |

</div>

---

## 🏗️ Architecture

```
Client (React + Tailwind v4)
        │  REST + Socket.IO
        ▼
Express API  →  Controllers  →  Services  →  PostgreSQL
        │
        ▼
  Google Gemini API  (backlog generation · task breakdown · sprint summary)
```

Backend follows a clean **routes → controllers → services** pattern with raw parameterized SQL,
centralized error handling, and JWT-protected routes. Every board/column/task query is scoped through
board membership — never trusted from the client — for true multi-tenant isolation.

---

## 📸 Screenshots

> _Add screenshots or a GIF of the board, drag-and-drop, and AI backlog generation here._

| Dashboard | Kanban Board | AI Backlog Generation |
|---|---|---|
| ![dashboard](docs/screenshots/dashboard.png) | ![board](docs/screenshots/board.png) | ![ai](docs/screenshots/ai-generate.png) |

---

## ⚙️ Getting Started

### Prerequisites
- Node.js ≥ 18
- PostgreSQL ≥ 14
- A Google Gemini API key ([get one here](https://ai.google.dev/))

### 1. Clone the repo
```bash
git clone https://github.com/your-username/ai-kanban-board.git
cd ai-kanban-board
```

### 2. Set up the backend
```bash
cd server
npm install
cp .env.example .env    # add your DB credentials, JWT secret & Gemini API key
npm run seed             # transactional, all-or-nothing seed script
npm run dev
```

### 3. Set up the frontend
```bash
cd client
npm install
npm run dev
```

### 4. Environment Variables (`server/.env`)
```env
DATABASE_URL=postgres://user:password@localhost:5432/ai_kanban
JWT_SECRET=your_jwt_secret
GEMINI_API_KEY=your_gemini_api_key
PORT=5000
```

The app will be running at `http://localhost:5173` (client) and `http://localhost:5000` (API).

---

## 📁 Project Structure

```
ai-kanban/
├── server/
│   ├── src/
│   │   ├── config/        # db pool, gemini client, socket instance
│   │   ├── middleware/     # auth, error handler, validation
│   │   ├── routes/         # thin route definitions
│   │   ├── controllers/    # request/response layer
│   │   ├── services/       # business logic + SQL
│   │   ├── sockets/        # real-time event handlers
│   │   ├── ai/              # Gemini prompt builders & parsers
│   │   └── db/              # schema.sql, seed.js
└── client/
    └── src/
        ├── api/             # axios wrappers
        ├── components/       # ui/, board/, dashboard/, layout/
        ├── hooks/            # useSocket, useAuth, useBoard
        ├── context/          # AuthContext, SocketContext
        └── pages/            # Dashboard, BoardView, MyTasks, Calendar, Team
```

---

## 🗺️ Roadmap

- [ ] Recurring tasks & sprint templates
- [ ] Slack/Discord notifications for board activity
- [ ] File attachments on tasks
- [ ] Dark mode
- [ ] Mobile app (React Native)

---

## 🤝 Contributing

Contributions are welcome! Please open an issue first to discuss what you'd like to change, then submit a PR.

1. Fork the repo
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📄 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

<div align="center">

### 💚 Built with the PERN stack, real-time sockets, and a little help from AI

**[Live Demo](#)** · **[Report Bug](../../issues)** · **[Request Feature](../../issues)**

</div>
