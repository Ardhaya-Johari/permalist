# 📝 Permalist – A Persistent To-Do Web App

![Permalist Banner]

**Permalist** is a simple yet powerful To-Do List web app built using **Node.js**, **Express**, **EJS**, and **PostgreSQL**. It lets users manage daily tasks — with functionality to **add**, **edit**, and **delete** items — all stored permanently in a PostgreSQL database.

---

## 🚀 Features

- ✅ Add new tasks
- 📝 Edit existing tasks inline
- ❌ Delete tasks via checkbox
- 📦 PostgreSQL for persistent storage
- ⚡ Fast and minimalistic interface using EJS templates
- 🎯 Smooth UX with clear task feedback

---

## 🛠️ Tech Stack

| Layer        | Technology             |
|--------------|------------------------|
| Backend      | Node.js, Express.js    |
| Database     | PostgreSQL (`pg` module) |
| Frontend     | EJS, HTML, CSS, JS     |
| Hosting      | Runs locally on `localhost:3000` |

---

## 📁 Project Structure

permalist/
├── public/ # Static assets (CSS, images)
├── views/ # EJS templates
│ ├── index.ejs
│ └── partials/
├── app.js # Main application server
├── package.json
├── README.md


---

## 📦 Getting Started

### 1. Clone the Repo

-git clone https://github.com/your-username/permalist.git
-cd permalist

### 2. Install Dependencies
-npm install

### 3.  Set Up PostgreSQL
-CREATE DATABASE permalist;

-CREATE TABLE items (
 id SERIAL PRIMARY KEY,
  title TEXT NOT NULL
);

### 4. Configure Your DB Credentials
-const db = new pg.Client({
  user: "your_pg_username",
  host: "localhost",
  database: "permalist",
  password: "your_pg_password",
  port: 5432,
});

### 5. Run the index.js
-npm index.js

## 🧠 How It Works
/ → Displays the list of items from PostgreSQL

/add → Adds a new item

/edit → Updates an existing item

/delete → Removes an item

### 🔮 Future Ideas
-✅ Task due dates and reminders

-🧩 User login & personal task lists

-📊 Dashboard with task analytics

-📱 PWA support for mobile devices

### 👩‍💻 Author
- Ardhaya Johari – Full Stack Developer
- 📧 ardhayasaxena3897@gmail.com
- 🌐 LinkedIn
- 💻 GitHub

- <i>"I drink chai while fixing bugs." </i>☕

