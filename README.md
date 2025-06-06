# Unsungfields AI Platform

This repository contains the full-stack AI platform developed in VS Code, with both **frontend** and **backend**.

---

##  Folder Structure

Unsungfields-AI/
 backend/          # FastAPI backend
 frontend/         # React + Vite frontend
 .gitignore
 README.md

---

##  How to Run Locally

### 1. Backend (FastAPI)

cd backend
python -m venv venv
venv\Scripts\activate         # For Windows
# Or source venv/bin/activate for Linux/macOS
pip install -r requirements.txt
uvicorn main:app --reload

### 2. Frontend (React + Vite)

cd frontend/vite-project
npm install
npm run dev

---

##  Required Dependencies

Make sure these are installed:

- Python 3.10+
- Node.js v18+
- MongoDB (local or remote)
- Redis Server (see below)

---

##  How to Install Redis on Windows (via WSL)

1. Open your WSL terminal (Ubuntu preferred):

sudo apt update
sudo apt install redis-server

2. Start Redis:

sudo service redis-server start

3. Test Redis:

redis-cli ping
# Output should be: PONG

> Redis runs on localhost:6379 by default.

---

##  Environment Variables

Create a `.env` file in your backend/ directory based on the example below:

### Example: backend/.env.example

REDIS_HOST=localhost
REDIS_PORT=6379
MONGO_URI=mongodb://localhost:27017/
SECRET_KEY=your-secret-key

---

##  Features

- Google & Email Authentication
- API Key Management
- Model Inference (Groq/Tenstorrent)
- Playground UI
- Token & Usage Tracking
- Redis-based Rate Limiting
