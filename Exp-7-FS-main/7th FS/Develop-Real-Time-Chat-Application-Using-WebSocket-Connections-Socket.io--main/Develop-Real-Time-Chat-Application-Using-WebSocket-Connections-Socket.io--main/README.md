# 💬 Real-Time Chat Application

A simple **real-time chat application** built using **React (frontend)** and **Node.js + Socket.IO (backend)**.

---

## 🚀 Features Implemented

✅ Real-Time Messaging – Instant updates using WebSockets  
✅ Join & Leave Notifications – System messages show user activity  
✅ Usernames – Each message tagged with sender’s name  
✅ Auto-Scroll – Latest messages always visible  
✅ Simple UI – Clean, responsive chat interface built with TailwindCSS  
✅ Custom Simulation (for frontend-only mode) – Works even without backend connection  

---

## 🛠️ Installation

### 1️⃣ Backend Setup (Chat Server)

```bash
npm init -y
npm install express socket.io cors
node server.js
```

Server will start at:
```
http://localhost:4000
```

### 2️⃣ Frontend Setup (React App)

Install dependencies and start development server:

```bash
npm install
npm start
```

---

## 📂 File Structure

```
chat-app/
├── server.js          # Express + Socket.IO backend
├── src/
│   └── ChatApp.js     # React frontend component
└── package.json
```

## 💡 Explanation

### Backend (server.js)
- Uses **Express** and **Socket.IO** for WebSocket communication.
- Handles events: `join`, `sendMessage`, and `disconnect`.
- Broadcasts system messages and chat updates to all connected clients.

### Frontend (ChatApp.js)
- React UI for joining chat and sending messages.
- Simulated socket behavior (if backend unavailable).
- Auto-scrolls to latest message.

---

---

## ⚡ Output Preview

### /OUTPUT/OUTPUT 1.png
![Output](OUTPUT/OUTPUT%201.png)

---

## ✅ Summary

| Layer | Tech Stack | Purpose |
|-------|-------------|----------|
| Backend | Node.js, Express, Socket.IO | Real-time server |
| Frontend | React + TailwindCSS | Chat UI |
| Communication | WebSocket (Socket.IO) | Instant message updates |

---

## 🎯 Result

You can chat in **real-time** between multiple browser tabs or users.  
Messages, join notifications, and disconnects all appear instantly.
