
# CI/CD Pipeline with GitHub Actions & Docker

This project demonstrates a complete CI/CD pipeline using GitHub Actions and Docker to build and deploy a simple static website.

## 🔧 Tools Used
- GitHub Actions
- Docker
- Docker Hub
- NGINX
- HTML/CSS

## 📁 Project Structure
```
.
├── app/
│   └── index.html
├── Dockerfile
├── .github/
│   └── workflows/
│       └── docker-ci.yml
```

## ⚙️ GitHub Actions Workflow
This workflow:
1. Builds a Docker image from `Dockerfile`
2. Pushes the image to Docker Hub
3. Can be deployed locally using Docker

### 🔑 GitHub Secrets Required:
- `DOCKER_USERNAME`
- `DOCKER_PASSWORD` (Docker Hub Access Token)

## 🐳 Docker Image
- [Docker Hub Repository](https://hub.docker.com/r/polankisravya/cicd-demo)

## 🧪 How to Run Locally
```bash
docker pull polankisravya/cicd-demo:latest
docker run -d -p 8080:80 polankisravya/cicd-demo:latest
```
Then open [http://localhost:8080](http://localhost:8080)

## ![image](https://github.com/user-attachments/assets/a616a9d1-e210-44af-a5d9-01aa5cefffd1)

- [GitHub Actions Success](https://github.com/polankisravya/CICD-pipeline/actions)
- [Docker Hub Image](https://hub.docker.com/r/polankisravya/cicd-demo)
- [Local App View](http://localhost:8080)

## 📄 Report
A 2-page PDF project report is included in the repo.
