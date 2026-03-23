# 🚀 CI/CD Pipeline for Node.js Dockerized Application

---

## 📌 Project Title
Automated CI/CD Pipeline using GitHub Actions and Docker

---

## 🎯 Objective
The goal of this project is to build a fully automated CI/CD pipeline that:
- Integrates code changes automatically  
- Builds and tests the application  
- Creates a Docker image  
- Pushes the image to Docker Hub  

This reduces manual effort and ensures faster, reliable deployments.

---

## 🛠️ Tools & Technologies Used
- **Version Control:** GitHub  
- **CI/CD Tool:** GitHub Actions  
- **Backend:** Node.js (Express)  
- **Containerization:** Docker  
- **Container Registry:** Docker Hub  

---

## 📁 Project Structure

CI-CD-project/
├── .github/
│ └── workflows/
│ └── ci-cd.yml
├── app.js
├── package.json
├── Dockerfile
└── node_modules/


---

## 🔄 CI/CD Pipeline Workflow

### 🔹 Trigger
- Pipeline starts automatically when code is pushed to the **main branch**

### 🔹 Build Stage (CI)
- Checkout repository code  
- Install dependencies (`npm install`)  
- Run tests (`npm test`)  

### 🔹 Package Stage (CD)
- Build Docker image  
- Tag image with Docker Hub username  
- Push image to Docker Hub  

---

## ⚙️ Workflow Flow

Developer → Git Push → GitHub Actions
→ Build & Test → Docker Build
→ Push to Docker Hub


---

This project demonstrates how DevOps practices can automate the software development lifecycle, making the process faster, reliable, and efficient.
