# Pawn Me Freak ♟️

A fully functional chess game with:
- React (Vite) frontend
- Node.js + Socket.IO backend (real-time)
- Online 2‑player matches with live chat
- Offline vs. Bot mode
- Colorful UI and capture splash with 
- Win/Lose toasts
- Auto-suggest chat lines

## Quick Start

### 1) Start the Backend
```bash
cd server
npm install
npm start
```
By default this runs on **http://localhost:4000**.

### 2) Start the Frontend
Open a new terminal:
```bash
cd client
npm install
npm run dev
```
Vite will show a local URL (usually **http://localhost:5173**). Open it in two browser windows to simulate two players.

> If you want to change the backend URL, edit `client/src/lib/socket.js`.

---

## Features

- **Lobby**: Create a room or join with a room code to play online.
- **Chat**: Real-time messages and auto-suggest buttons.
- **Board**: Valid move highlighting, turn indicator, capture splash (👅💦).
- **Server-side validation**: Moves are validated with `chess.js` on the server to prevent cheating.
- **Offline Bot**: Play vs. a simple bot that picks a reasonable (but beatable) move.

---

## Project Structure

```
pawn-me-freak/
├─ server/               # Node.js + Socket.IO backend
│  ├─ index.js
│  └─ package.json
└─ client/               # React (Vite) frontend
   ├─ index.html
   ├─ package.json
   ├─ vite.config.js
   └─ src/
      ├─ main.jsx
      ├─ App.jsx
      ├─ styles.css
      ├─ lib/
      │  ├─ socket.js
      │  └─ bot.js
      └─ components/
         ├─ Lobby.jsx
         ├─ Board.jsx
         ├─ Square.jsx
         ├─ Chat.jsx
         └─ EmojiSplash.jsx
```

---

## Notes
- Tested on Node 18+.
- If ports conflict, change `PORT` in `server/index.js` and `VITE_SERVER_URL` in `client/.env` (create it) or directly in `client/src/lib/socket.js`.
- This is intentionally playful and vibrant, per your request.
