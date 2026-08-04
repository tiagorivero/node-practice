# Real-Time Chat

> 🚧 Work in progress — this project is still being built.

A real-time chat app built with Node.js, Express, and Socket.IO to practice WebSocket communication.

## Features (so far)

- Real-time messaging between connected clients
- Simple chat UI with message list and input form
- Server logs for connections/disconnections (via morgan)

## Planned / not implemented yet

- Usernames / identifying who sent each message
- Message persistence
- Styling improvements

## Tech stack

- Node.js
- Express
- Socket.IO
- Morgan (HTTP request logging)

## Backend concepts practiced

- Real-time, bidirectional communication with WebSockets (Socket.IO)
- Event-based server architecture (`connection`, `disconnect`, custom events)
- Serving a static HTML client from Express

## Run locally

Clone the repository and install the dependencies:

```bash
npm install
```

Start the server:

```bash
node index.js
```

Open `http://localhost:3000` in your browser. Open it in multiple tabs to test the real-time chat.