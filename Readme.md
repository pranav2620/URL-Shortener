# 🔗 URL Shortener System

A full-stack web application that converts long URLs into short, shareable links with persistent storage and click analytics. Built using Node.js, Express, MongoDB, and EJS.

---

## 🖼️ Application Preview

### 🔹 Home Interface
![Home](images/home.png)

### 🔹 URL Shortening in Action
![Shorten](images/shorten.png)

### 🔹 Multiple URLs Stored
![Multiple URLs](images/multiple.png)

---

## ⚙️ System Architecture

![Architecture](images/architecture.png)

The application follows a client-server architecture:

- **Client** → Sends requests (URL input, redirect, delete)
- **Server (Express.js)** → Handles routing and logic
- **Database (MongoDB)** → Stores URL mappings and analytics

---

## 🔄 Workflow

### 1️⃣ URL Shortening
![Shortening Flow](images/shortening_flow.png)

- User submits a long URL  
- Server generates a short ID  
- Stores mapping in database  
- Displays shortened URL  

---

### 2️⃣ Redirection
![Redirection Flow](images/redirection_flow.png)

- User clicks short URL  
- Server retrieves original URL  
- Increments click count  
- Redirects user  

---

### 3️⃣ Deletion
![Deletion Flow](images/deletion_flow.png)

- User deletes a URL  
- Server removes entry from database  
- Updated list is displayed  

---

## 🗄️ Database Schema

![Schema](images/schema.png)

| Field   | Type   | Description                     |
|--------|--------|---------------------------------|
| full   | String | Original URL                   |
| short  | String | Shortened unique ID            |
| clicks | Number | Number of visits               |

---

## 🛠️ Tech Stack

- **Backend:** Node.js, Express.js  
- **Database:** MongoDB, Mongoose  
- **Frontend:** HTML, Bootstrap, EJS  
- **Utility:** shortid  

---

## 🧑‍💻 Setup & Execution

### 🔹 MongoDB Connection
![MongoDB](images/mongo.png)

### 🔹 Run Server
![Terminal](images/server.png)

```bash
npm install
npm start
```

---

## 🌐 Live Working Demo

### URL Creation & Storage
![Demo1](images/demo1.png)

### Click Tracking
![Demo2](images/demo2.png)

### Redirection Example
![Redirect](images/redirect.png)

### Delete Functionality
![Delete](images/delete.png)

---

## 🚀 Features

- URL shortening with unique IDs  
- Redirection handling  
- Click tracking (analytics)  
- Delete functionality  
- Persistent storage  

---

## ⚠️ Limitations

- No authentication  
- No URL validation  
- No custom aliases  
- Single server (not scalable yet)  

---

## 🔮 Future Enhancements

- User authentication (JWT)  
- Custom short URLs  
- Expiry links  
- Rate limiting  
- Redis caching  
- Analytics dashboard  

---

## 📌 Learning Outcomes

- Backend routing with Express  
- Database schema design (MongoDB)  
- RESTful architecture  
- Request-response lifecycle  
- System design fundamentals  

---

## 📎 Acknowledgment

Inspired by system design concepts from URL shortening services like Bitly and TinyURL.
