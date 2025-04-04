# Unsungfields AI Platform

This repository contains the full-stack AI platform developed in VS Code, with both **frontend** and **backend**.

##  Folder Structure
``Unsungfields-AI/
 backend/          # FastAPI backend
 frontend/         # React + Vite frontend
 .gitignore
 README.md
``

##  How to Run Locally

### 1. Backend (FastAPI)
`ash
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
` 

### 2. Frontend (React + Vite)
`ash
cd frontend/vite-project
npm install
npm run dev
` 

##  Features
- Google & Email Authentication
- API Key Management
- Model Inference (via Groq/Tenstorrent)
- Playground Interface
