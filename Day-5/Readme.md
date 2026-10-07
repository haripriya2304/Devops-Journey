# 🐳 Docker Custom Images & GitHub Container Registry

Hands-on practice with building custom Docker images and pushing them to **GitHub Container Registry (GHCR)**.

## 📌 Topics Covered

- Creating and working with a `Dockerfile`
- Building custom Docker images
- Docker image tagging
- Logging in to GitHub Container Registry
- Tagging images for GHCR
- Pushing images to GHCR
- Troubleshooting Docker image naming

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

## 🔄 Workflow

```text
Dockerfile
    ↓
docker build
    ↓
Docker Image
    ↓
docker login
    ↓
docker tag
    ↓
docker push
    ↓
GitHub Container Registry
```

## 🎯 Key Learnings

- Built custom Docker images using a `Dockerfile`
- Learned Docker image names and tags
- Authenticated with GHCR
- Tagged and pushed images to GHCR
- Learned to troubleshoot `No such image` errors

## 👩‍💻 Author

**Haripriya V**  
B.E. Computer Science & Engineering  
**Aspiring Software Engineer | Cloud Enthusiast**
