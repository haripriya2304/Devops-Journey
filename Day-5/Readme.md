# 🐳 Docker Custom Images, GHCR & Jenkins Integration

Hands-on practice with **Docker custom images, GitHub Container Registry (GHCR), and Jenkins CI/CD integration with Git and Docker**.

## 📌 Topics Covered

- Creating and working with a `Dockerfile`
- Building custom Docker images
- Docker image tagging
- Pushing images to GitHub Container Registry
- Git & Jenkins integration
- Jenkins & Docker integration
- Automating Docker image builds using Jenkins

## 🛠️ Commands Practiced

```bash
# Build Docker image
docker build -t customimg:latest .

# List Docker images
docker images

# Login to GHCR
docker login ghcr.io -u haripriya2304

# Tag image for GHCR
docker tag jenkinstest:latest ghcr.io/haripriya2304/jenkinstest:latest

# Push image to GHCR
docker push ghcr.io/haripriya2304/jenkinstest:latest
```

## 🔄 Jenkins CI/CD Workflow

```text
Git Repository
      ↓
   Jenkins
      ↓
  Pull Source Code
      ↓
   Docker Build
      ↓
 Docker Image
      ↓
   Docker Push
      ↓
GitHub Container Registry
```

## 🎯 Key Learnings

- Built custom Docker images using Dockerfile
- Learned Docker image tagging and pushing
- Worked with GitHub Container Registry
- Integrated **Git with Jenkins**
- Integrated **Jenkins with Docker**
- Automated Docker image building through Jenkins
- Understood the basics of a CI/CD pipeline

## 👩‍💻 Author

**Haripriya V**  
B.E. Computer Science & Engineering  
**Aspiring Software Engineer | Cloud Enthusiast**
