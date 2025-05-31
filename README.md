# 🗒️ Quick-Stick

**Quick-Stick** is a lightweight sticky notes web app built with pure HTML, CSS, and JavaScript. It lets you create, move, edit, and delete sticky notes directly in the browser. Ideal for quick note-taking without any login or backend.

🔗 **Live Demo:** [quick-stick.vercel.app](https://quick-stick.vercel.app)

---

## ✨ Features

- 📝 Create, edit, and delete sticky notes
- 📌 Drag-and-drop positioning
- 💾 Persistent local storage
- ⚡ Blazing fast and minimalist

---

## 📁 Project Structure

```
Quick-Stick/
├── index.html         # Main HTML file
├── style.css          # Stylesheet
├── script.js          # JavaScript logic
├── docker-compose.yaml
└── assets/            # Static assets (e.g., icons)
```

---

## 🚀 Getting Started

### 🔧 Manual Setup (Without Docker)

1. Clone the repository:

   ```bash
   git clone https://github.com/vinayak-jaybhaye/Quick-Stick.git
   cd Quick-Stick
   ```

2. Open `index.html` in your browser:
   ```bash
   open index.html
   ```

---

### 🐳 Run with Docker

> Make sure you have Docker and Docker Compose installed.

1. Clone the repository:

   ```bash
   git clone https://github.com/vinayak-jaybhaye/Quick-Stick.git
   cd Quick-Stick
   ```

2. Start the app using Docker Compose:

   ```bash
   docker-compose up
   ```

3. Open your browser and go to [http://localhost:3000](http://localhost:3000)

---

## 📦 Docker Compose Overview

The app uses an Nginx container to serve the static files.

**docker-compose.yaml**

```yaml
services:
  web:
    image: nginx:alpine
    ports:
      - "3000:80"
    volumes:
      - ./:/usr/share/nginx/html:ro

```

---

## 📝 License

This project is licensed under the [MIT License](LICENSE).
