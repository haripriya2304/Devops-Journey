# 🐳 Docker Basics – Day 3

This repository contains my **Day 3 hands-on practice with Docker**, focusing on essential commands for working with Docker images and containers.

## 📌 Topics Covered

- Checking Docker version
- Searching Docker Hub for images
- Pulling Docker images
- Listing Docker images
- Creating containers
- Running containers
- Listing containers
- Starting containers
- Stopping containers
- Assigning custom names to containers
- Understanding the Docker container lifecycle

---

## 🛠️ Tools & Technologies

- **Docker**
- **Docker Hub**
- **Apache HTTP Server (`httpd`)**
- **Node.js Docker Image**
- **Windows PowerShell**

---

# 🚀 Getting Started

Make sure Docker is installed and Docker Desktop is running.

Check the Docker installation using:

```bash
docker -v
```

Example output:

```text
Docker version 28.x.x
```

---

# 📦 Docker Images

A **Docker image** is a read-only template used to create Docker containers.

## 1. Search for an Image

```bash
docker search <image-name>
```

Searches Docker Hub for available images.

Example:

```bash
docker search node
```

---

## 2. Pull an Image

```bash
docker pull <image-name>
```

Downloads an image from Docker Hub to the local system.

Example:

```bash
docker pull node
```

---

## 3. Pull Apache HTTP Server Image

```bash
docker pull httpd
```

Downloads the official Apache HTTP Server image.

The `httpd` image can later be used to create containers running Apache HTTP Server.

---

## 4. List Docker Images

```bash
docker images
```

Displays all Docker images available locally.

Example:

```text
REPOSITORY   TAG       IMAGE ID       CREATED       SIZE
httpd        latest    xxxxxxxx       ...           ...
node         latest    xxxxxxxx       ...           ...
```

---

# 📦 Docker Containers

A **container** is a running or stopped instance created from a Docker image.

## 5. Create a Container

```bash
docker create httpd
```

Creates a container from the `httpd` image.

The container is created but **not started**.

---

## 6. Run a Container

```bash
docker run httpd
```

The `docker run` command creates a new container and starts it immediately.

### Difference Between `docker create` and `docker run`

```text
docker create
      ↓
Creates a container
      ↓
Container remains stopped
```

Whereas:

```text
docker run
      ↓
Creates a container
      ↓
Starts the container
```

So:

> `docker run` = `docker create` + `docker start`

---

# 🔍 Viewing Containers

## 7. View Running Containers

```bash
docker ps
```

Displays only the containers that are currently running.

---

## 8. View All Containers

```bash
docker ps -a
```

Displays all containers, including:

- Running containers
- Stopped containers
- Created containers

---

# ▶️ Starting and Stopping Containers

## 9. Start a Container

```bash
docker start <container-name>
```

Starts an existing stopped container.

Example:

```bash
docker start democon
```

---

## 10. Stop a Container

```bash
docker stop <container-name>
```

Stops a running container.

Example:

```bash
docker stop democon
```

---

# 🏷️ Naming Containers

Docker automatically generates a random name when a container is created without specifying one.

We can assign our own name using the `--name` option.

## 11. Create a Named Container

```bash
docker create --name democon httpd
```

This creates a container from the `httpd` image and assigns it the name:

```text
democon
```

The container can then be managed using its custom name.

For example:

```bash
docker start democon
```

and:

```bash
docker stop democon
```

---

# 🔄 Docker Container Lifecycle

The basic Docker container lifecycle practiced in this session:

```text
                Docker Image
                     │
                     ▼
              docker create
                     │
                     ▼
             Container Created
                     │
                     ▼
               docker start
                     │
                     ▼
            Running Container
                     │
                     ▼
               docker stop
                     │
                     ▼
            Stopped Container
```

Using `docker run`:

```text
                Docker Image
                     │
                     ▼
                 docker run
                     │
                     ▼
          Container Created
                     │
                     ▼
          Container Started
                     │
                     ▼
          Running Container
```

---

# 📋 Docker Command Reference

| Command | Description |
|---|---|
| `docker -v` | Check Docker version |
| `docker search <image>` | Search Docker Hub for images |
| `docker pull <image>` | Download an image |
| `docker images` | List local Docker images |
| `docker create <image>` | Create a container without starting it |
| `docker run <image>` | Create and start a container |
| `docker ps` | List running containers |
| `docker ps -a` | List all containers |
| `docker start <container>` | Start a stopped container |
| `docker stop <container>` | Stop a running container |
| `docker create --name <name> <image>` | Create a container with a custom name |

---

# 🧪 Practice Workflow

The following workflow summarizes the commands practiced:

```bash
# Check Docker version
docker -v

# Search for an image
docker search node

# Pull an image
docker pull node

# Pull Apache HTTP Server image
docker pull httpd

# List available images
docker images

# Create a container
docker create httpd

# Run a container
docker run httpd

# View running containers
docker ps

# View all containers
docker ps -a

# Create a named container
docker create --name democon httpd

# Start the container
docker start democon

# Stop the container
docker stop democon
```

---

# 🎯 Key Learnings

Through this hands-on practice, I learned:

- How Docker images and containers work
- How to check the Docker installation
- How to search for images on Docker Hub
- How to download Docker images
- How to list locally available images
- How to create containers
- How to run containers
- The difference between `docker create` and `docker run`
- How to view running and stopped containers
- How to start and stop containers
- How to assign custom names to containers
- The basic lifecycle of a Docker container

---

# 📚 Concepts

### Docker Image

A Docker image is a packaged, read-only template containing everything required to create a container.

### Docker Container

A container is an isolated runtime environment created from a Docker image.

### Docker Hub

Docker Hub is a registry where Docker images can be stored, searched, and downloaded.

### `docker run`

Creates and starts a new container from an image.

### `docker create`

Creates a container without starting it.

### `docker start`

Starts an existing stopped container.

### `docker stop`

Stops a running container.

---

# 👩‍💻 Author

**Haripriya V**

B.E. Computer Science & Engineering

---

## 📈 Learning Journey

This is part of my hands-on **Cloud & DevOps learning journey**, where I am building practical knowledge of Docker, containers, Kubernetes, and other DevOps technologies.
