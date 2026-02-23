# MEAN Stack Docker Deployment

## 📌 Project Overview

This project is a full-stack CRUD application built using the MEAN stack:

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

## 🏗 Architecture

Frontend (Angular) → Backend (Node + Express API) → MongoDB

The application is containerized using Docker and deployed on an Ubuntu VM using Docker Compose. CI/CD is implemented using GitHub Actions, and Nginx is configured as a reverse proxy.

---

## 🖥 Local Development Setup

### Backend

```bash
cd backend
npm install
node server.js
