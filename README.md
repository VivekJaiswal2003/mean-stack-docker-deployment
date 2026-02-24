# MEAN Stack CRUD Application (Production Ready)

This project is a full-stack CRUD application built using the **MEAN Stack**:

- MongoDB
- Express.js
- Angular 15
- Node.js

The application manages tutorials with the following fields:

- id
- title
- description
- published status

Users can:

- Create tutorials
- Retrieve tutorials
- Update tutorials
- Delete tutorials
- Search tutorials by title

---

## 🌍 Live Deployment

🔗 **Live Demo:**  
http://3.90.16.24

---

## 🏗 Architecture

Frontend (Angular)  
⬇  
Backend (Node.js + Express REST API)  
⬇  
MongoDB Database  

The frontend communicates with the backend API, which interacts with MongoDB.

---

## 🐳 Containerization

The entire application is containerized using Docker:

- Backend Dockerfile
- Frontend Dockerfile (Multi-stage build with Nginx)
- MongoDB official image

Docker Compose is used to orchestrate:

- Frontend
- Backend
- MongoDB

---

## ☁ Cloud Deployment

The application is deployed on:

- AWS EC2 (Ubuntu Server)
- Docker & Docker Compose
- Public HTTP access via Port 80

Security configuration:
- Backend and MongoDB are internal services
- Only port 80 (HTTP) is publicly exposed

---

## 🔄 CI/CD Pipeline

CI/CD is implemented using **GitHub Actions**.

Pipeline Workflow:

1. Code pushed to GitHub
2. Docker images built automatically
3. Images pushed to Docker Hub
4. Deployment updated on EC2

---

## 🖥 Local Development Setup

### Backend

```bash
cd backend
npm install
node server.js
node server.js
