# 🚀 Docker Hub Registry Management & Container Image Deployment

![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Docker Hub](https://img.shields.io/badge/Docker%20Hub-Registry-blue)
![DevOps](https://img.shields.io/badge/DevOps-Practice-orange)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)

---

# 📌 Project Overview

This project demonstrates the complete Docker image lifecycle, from building a custom Docker image to publishing it on Docker Hub and redeploying it from the registry.

The project was created as a hands-on DevOps and Cloud Computing lab to gain practical experience with:

✅ Docker Containers

✅ Docker Images

✅ Docker Hub Registry

✅ Image Tagging & Versioning

✅ Container Deployment

✅ Nginx Web Server

✅ DevOps Best Practices

The project simulates a real-world workflow used by DevOps Engineers, Cloud Engineers, Site Reliability Engineers (SREs), and Platform Engineers.

---

# 🎯 Objectives

- Create a custom Docker image
- Containerize a static web application
- Build images using Dockerfile
- Run and manage Docker containers
- Push images to Docker Hub
- Pull images from Docker Hub
- Understand image versioning
- Practice registry management
- Learn deployment workflow

---

# 🏗️ Project Architecture

```text
Developer
    │
    ▼
Source Code
(index.html)
    │
    ▼
Dockerfile
    │
    ▼
Docker Build
    │
    ▼
Docker Image
(mywebsite)
    │
    ▼
Docker Hub Repository
    │
    ▼
Docker Pull
    │
    ▼
Container Deployment
    │
    ▼
Web Application
```

---

# 📂 Repository Structure

```text
DockerHub-Lab/
│
├── index.html
│
├── Dockerfile
│
├── screenshots/
│
└── README.md
```

---

# 💻 Technologies Used

- Docker
- Docker Hub
- Nginx
- HTML
- Windows PowerShell
- VS Code

---

# 📄 Application Source Code

## index.html

```html
<!DOCTYPE html>
<html>
<head>
    <title>Docker Hub Lab</title>
</head>
<body>
    <h1>Hello From Docker Hub Project</h1>
</body>
</html>
```

---

# 🐳 Dockerfile

```dockerfile
FROM nginx

COPY index.html /usr/share/nginx/html/index.html
```

---

# 🔨 Build Docker Image

```bash
docker build -t mywebsite .
```

---

# ▶️ Run Container

```bash
docker run -d -p 8081:80 mywebsite
```

---

# 🌐 Access Application

```text
http://localhost:8081
```

Expected Output:

```text
Hello From Docker Hub Project
```

---

# 🏷️ Tag Docker Image

```bash
docker tag mywebsite <dockerhub-username>/mywebsite:v1
```

Example:

```bash
docker tag mywebsite niteshvishwakarma/mywebsite:v1
```

---

# ☁️ Push Image to Docker Hub

```bash
docker push niteshvishwakarma/mywebsite:v1
```

---

# 📥 Pull Image from Docker Hub

```bash
docker pull niteshvishwakarma/mywebsite:v1
```

---

# 🔄 Container Lifecycle Commands

## View Running Containers

```bash
docker ps
```

## View All Containers

```bash
docker ps -a
```

## View Images

```bash
docker images
```

## Stop Container

```bash
docker stop <container-id>
```

## Remove Container

```bash
docker rm <container-id>
```

## Remove Image

```bash
docker rmi <image-id>
```

---

# 📚 Learning Outcomes

After completing this project, I gained practical experience in:

✔ Docker Installation & Configuration

✔ Docker Image Creation

✔ Docker Container Management

✔ Dockerfile Authoring

✔ Docker Hub Registry Operations

✔ Image Versioning

✔ Container Deployment

✔ DevOps Workflow

✔ Registry-Based Application Distribution

✔ Industry Standard Container Practices

---

# 🎯 Real-World Use Cases

- Application Packaging
- CI/CD Pipelines
- Cloud Deployments
- Kubernetes Workloads
- Microservices Deployment
- DevOps Automation
- Container-Based Infrastructure

---

# 🏆 Resume Highlights

- Built and deployed custom Docker containers using Docker Engine.
- Created Docker images using Dockerfile and Nginx.
- Managed image versioning and repository publishing on Docker Hub.
- Performed container deployment, image distribution, and registry management.
- Demonstrated hands-on DevOps practices using Docker and Docker Hub.

---

# 👨‍💻 Author

**Nitesh Vishwakarma**

BCA (Cloud & Security)

Aspiring Cloud Engineer | DevOps Engineer | AWS Practitioner

---

⭐ If you found this project useful, consider giving it a star.
