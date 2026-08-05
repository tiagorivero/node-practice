# Real-Time Chat

A real-time chat app built with Node.js, Express, and Socket.IO, with persistent message history using Turso (libSQL).

<img width="461" height="821" alt="Image" src="https://github.com/user-attachments/assets/a426701b-5f89-41ef-837a-ebe6e4ef35b5" />

## Features

- Real-time messaging between connected clients
- Messages persisted in a database (Turso / libSQL)
- Message history recovery on reconnect, using Socket.IO's connection state recovery
- Random usernames auto-assigned per client (via the Random User API) and remembered with localStorage
- Auto-scroll to the latest message

## Tech stack

- Node.js
- Express
- Socket.IO
- Turso (libSQL) — database
- dotenv
- Morgan (HTTP request logging)

## Backend concepts practiced

- Real-time, bidirectional communication with WebSockets (Socket.IO)
- Connection state recovery to resend missed messages after a disconnect
- Persisting and querying data with a SQL database (libSQL/Turso)
- Environment variables for sensitive credentials

## Setup

This project needs a Turso database to store chat messages.

1. Create a free database at [turso.tech](https://turso.tech/)
2. Create a `.env` file in the project root and add:

```
DB_URL=your_turso_database_url_here
DB_TOKEN=your_turso_auth_token_here
```

## Run locally

Clone the repository and install the dependencies:

```bash
npm install
```

Start the server:

```bash
node server/index.js
```

Open `http://localhost:3000` in your browser. Open it in multiple tabs to test the real-time chat.
