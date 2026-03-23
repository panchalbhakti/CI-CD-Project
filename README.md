### CI-CD Project

# 🚀 CI/CD Pipeline for Node.js Dockerized Application

![CI/CD](https://github.com/panchalbhakti/CI-CD-Project/actions/workflows/ci-cd.yml/badge.svg)

## 📌 Project Title
Automated CI/CD Pipeline using GitHub Actions and Docker

## 🎯 Objective
The goal of this project is to build a fully automated CI/CD pipeline that:

Integrates code changes automatically
Builds and tests the application
Creates a Docker image
Pushes the image to Docker Hub

This reduces manual effort and ensures faster, reliable deployments.

## 🛠️ Tools & Technologies
Version Control: GitHub
CI/CD Tool: GitHub Actions
Backend: Node.js (Express)
Containerization: Docker
Container Registry: Docker Hub

## 📁 Project Structure
```
CI-CD-project/
├── .github/
│   └── workflows/
│       └── ci-cd.yml       # CI/CD workflow file
├── app.js                 # Main application file
├── package.json           # Dependencies & scripts
├── Dockerfile             # Docker configuration
└── node_modules/
```

## 🔄 CI/CD Pipeline Flow
```
🔹 Trigger
Pipeline starts automatically when code is pushed to the main branch
🔹 Build Stage (CI)
Checkout repository code
Install dependencies (npm install)
Run tests (npm test)
🔹 Package Stage (CD)
Build Docker image
Tag image with Docker Hub username
Push image to Docker Hub
```

## 🚀 Pipeline Stages
- **Source Stage:** Code committed to GitHub repository
- **Trigger:** Push to main branch triggers GitHub Actions
- **Build Stage:** Checkout code, install dependencies, run tests
- **Package Stage:** Build Docker image and push to Docker Hub
- **Artifact:** Container image available on Docker Hub

## ⚙️ How to Run Locally
```bash
# Install dependencies
npm install

# Run tests
npm test

# Start server
npm start
```

## 🐳 Docker
```bash
# Build image
docker build -t my-cicd-app .

# Run container
docker run -p 3000:3000 my-cicd-app

# Visit http://localhost:3000
```

## 🔐 GitHub Secrets Required
| Secret | Description |
|--------|-------------|
| DOCKER_USERNAME | Docker Hub username |
| DOCKER_PASSWORD | Docker Hub access token |

## ✅ Expected Output
A fully automated pipeline that ensures every code change is 
integrated, tested, and containerized, providing a deployable 
artifact on Docker Hub with minimal manual intervention.
