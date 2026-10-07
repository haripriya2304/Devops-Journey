# 🐳 Docker Compose – Day 4

This repository contains my **Day 4 hands-on practice with Docker**, focusing on **Docker Compose** and managing multi-container applications using a `docker-compose.yml` file.

## 📌 Topics Covered

- Introduction to Docker Compose
- Creating a Docker Compose YAML file
- Running multi-container applications
- Starting and stopping services
- Viewing Compose containers
- Viewing images used by Compose
- Working with Docker networks
- Running containers in detached mode
- Creating and serving a frontend using Docker Compose
- Understanding the Docker Compose workflow

---

## 🛠️ Tools & Technologies

- **Docker**
- **Docker Compose**
- **YAML**
- **HTML**
- **Linux Terminal**
- **Docker Networks**

---

# 🚀 What is Docker Compose?

**Docker Compose** is a tool used to define and run multi-container Docker applications.

Instead of running multiple `docker run` commands separately, we can define the application's services inside a YAML file and manage them using Docker Compose.

For example, an application may contain:

```text
Application
│
├── Frontend
├── Backend
└── Database
