![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&color=F15A24&width=600&lines=📝+Permalist+Project+-+Your+Personal+To-Do+Tracker;✅+Add%2C+Track%2C+Edit+Tasks+Easily;🚀+Organized+Tasks%2C+Simplified+Life)

# 📝 Permalist – A Persistent To-Do Web App


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

```
permalist/
├── public/             # Static assets (CSS, images)
├── views/              # EJS templates
│   ├── index.ejs
│   └── partials/
├── index.js              # Main application server
├── package.json
├── README.md
```

---

## 📦 Getting Started

### 1. Clone the Repo

```bash
git clone https://github.com/your-username/permalist.git
cd permalist
```

### 2. Install Dependencies

```bash
npm install
```

### 3. Set Up PostgreSQL

Ensure PostgreSQL is installed and running.

#### Create the Database

```sql
CREATE DATABASE permalist;
```

#### Create the Table

```sql
CREATE TABLE items (
  id SERIAL PRIMARY KEY,
  title TEXT NOT NULL
);
```

### 4. Configure Your DB Credentials

Open `index.js` and update this block:

```js
const db = new pg.Client({
  user: "your_pg_username",
  host: "localhost",
  database: "permalist",
  password: "your_pg_password",
  port: 5432,
});
```

### 5. Run the App

```bash
node index.js

---

## 🧠 How It Works

- `/` → Displays the list of items from PostgreSQL  
- `/add` → Adds a new item  
- `/edit` → Updates an existing item  
- `/delete` → Removes an item  

---

## 🔮 Future Ideas

- ✅ Task due dates and reminders  
- 🧩 User login & personal task lists  
- 📊 Dashboard with task analytics  
- 📱 PWA support for mobile devices  

---

## 👩‍💻 Author

**Ardhaya Johari** – Full Stack Developer  
📧 ardhayasaxena3897@gmail.com  
🌐 [LinkedIn](https://www.linkedin.com/in/ardhaya-johari-819275321/)  
💻 [GitHub](https://github.com/Ardhaya-Johari)  

> _"I drink chai while fixing bugs."_ ☕

---

## 📄 License

MIT License
