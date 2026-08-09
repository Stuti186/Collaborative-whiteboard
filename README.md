#  Real-Time Collaborative Whiteboard & Code Editor

A real-time collaborative workspace that allows multiple users to **draw, brainstorm, write code, and communicate together** in a shared environment. Changes are synchronized instantly across connected users using WebSockets.

##  Features

* **Interactive Whiteboard**

  * Draw freehand
  * Create shapes and diagrams
  * Add text and annotations
  * Erase and modify elements

* **Real-Time Collaboration**

  * Multiple users can work on the same board simultaneously
  * Changes are synchronized instantly
  * Room-based collaboration

*  **Collaborative Code Editor**

  * Write and edit code together
  * Real-time synchronization between users
  * Supports multiple programming languages

*  **Shareable Collaboration Rooms**

  * Create or join a workspace using a room ID
  * Invite other users to collaborate

*  **Real-Time Communication**

  * WebSocket-based communication
  * Low-latency updates between clients and server

*  **Responsive Interface**

  * Designed to work across different screen sizes

## Tech Stack

### Frontend

* React.js
* HTML5 Canvas
* CSS
* JavaScript

### Backend

* Node.js
* Express.js
* Socket.IO

### Database

* MongoDB

### Tools

* Git & GitHub
* VS Code
* npm


##  How Real-Time Collaboration Works

1. A user creates or joins a collaboration room.
2. The client establishes a Socket.IO connection with the server.
3. When a user draws or modifies the whiteboard, the client emits an event.
4. The server receives the event and broadcasts the update to other users in the same room.
5. Connected clients update their whiteboards instantly.
6. Similar synchronization is used for collaborative code editing.

```text
User A
   │
   │ Drawing / Code Change
   ▼
React Client
   │
   │ Socket.IO Event
   ▼
Node.js + Socket.IO
   │
   │ Broadcast
   ▼
┌───────────────┐
│ User B        │
│ User C        │
│ User D        │
└───────────────┘
```

##  Use Cases

*  Pair programming
*  Online teaching and learning
*  Brainstorming sessions
*  Team meetings
*  Collaborative diagramming

##  Why This Project?

This project demonstrates the implementation of **real-time distributed collaboration** using WebSockets. It combines frontend development, backend APIs, database management, and event-driven communication to create an interactive multi-user application.


---

⭐ If you found this project useful, consider giving it a star!
