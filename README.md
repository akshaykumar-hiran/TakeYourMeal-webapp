# 🍽️ TakeYourMeal – Full-Stack Restaurant App

A **full-stack restaurant web application** for exploring, listing, and managing a variety of delicious meals.  
Built with **React (Frontend)**, **Express.js (Backend)**, and **MongoDB (Database)**.  
Includes **Admin Panel** and **Docker** support for an all-in-one setup.

---

## ✨ Features

- 🛍 **User Frontend** – Browse and search meals with a clean UI.
- 🛠 **Admin Panel** – Manage meals, images, and categories.
- ⚡ **REST API** – Fast and scalable backend.
- 🐳 **Dockerized** – Ready-to-run with a single command.
- 📱 **Responsive UI** – Works across devices.

---

## 🖥 Tech Stack

| Layer       | Technologies Used |
|-------------|-------------------|
| **Frontend** | React 18, Vite, React Router DOM, ESLint |
| **Backend** | Node.js, Express.js, CORS, Multer |
| **Database** | MongoDB |
| **DevOps** | Docker, Docker Compose |

---

## 🚀 Quick Start

### **Option 1: Docker Setup (Recommended)**

```bash
# Clone repository
git clone https://github.com/your-username/takeyourmeal.git
cd takeyourmeal
npm install

# Start all services
docker-compose up --build
````

**Services & Ports**:

* 🌐 **Frontend** → [http://localhost:3000](http://localhost:3000)
* 🛠 **Admin Panel** → [http://localhost:5173](http://localhost:5173)
* 🔌 **Backend API** → [http://localhost:4000](http://localhost:4000)
* 🗄 **MongoDB** → `localhost:27017`

---

### **Option 2: Manual Setup**

#### Prerequisites:

* Node.js (v16+)
* npm or yarn
* MongoDB (local or cloud)

```bash
# Clone repository
git clone https://github.com/your-username/takeyourmeal.git
cd takeyourmeal

# Install dependencies for each service
cd frontend && npm install && cd ..
cd backend && npm install && cd ..
cd admin && npm install && cd ..
```

**Run Services:**

```bash
# Frontend
cd frontend && npm run dev

# Admin Panel
cd admin && npm run dev

# Backend
cd backend && npm run server

# MongoDB
mongod
```

---

## 📂 Project Structure

```
TakeYourMeal/
├── frontend/                 # React user interface
├── backend/                  # Express.js REST API
├── admin/                    # React admin dashboard
├── docker-compose.yml        # Docker service orchestration
└── README.md
```

---

## 🐳 Docker Commands

```bash
# Build & start
docker-compose up --build

# Start in background
docker-compose up -d

# Stop all services
docker-compose down

# Stop & remove volumes (⚠ Deletes database data)
docker-compose down -v

# Logs
docker-compose logs -f backend
```

---

## ⚙ Environment Variables

**Backend**

```env
MONGODB_URI=mongodb://admin:password123@mongodb:27017/takeyourmeal
JWT_SECRET=your_jwt_secret
PORT=4000
```

**Frontend**

```env
REACT_APP_API_URL=http://localhost:4000
```

**Admin**

```env
VITE_API_URL=http://localhost:4000
```

---

## 🧪 Linting

```bash
# Frontend
cd frontend && npm run lint

# Admin
cd admin && npm run lint
```

---

## 📜 License

Licensed under the **MIT License**. You are free to use, modify, and distribute this project.

---

## 🔗 References

* [React](https://reactjs.org/)
* [Vite](https://vitejs.dev/)
* [Express.js](https://expressjs.com/)
* [MongoDB](https://www.mongodb.com/)
* [Docker](https://www.docker.com/)

```
