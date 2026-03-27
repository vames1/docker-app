# 🐳 Dockerised Web Application

A complete Docker project featuring a custom Nginx web application with Docker Networking, Volumes, Docker Compose and automated CI/CD deployment to AWS ECS using GitHub Actions.

---

## 🏗️ Architecture
```
GitHub Push
    ↓
GitHub Actions CI/CD Pipeline
    ↓
Build Docker Image
    ↓
Push to Docker Hub
    ↓
Deploy to AWS ECS Fargate
    ↓
Live on AWS! 🚀
```

---

## 🚀 Technologies Used

| Technology | Purpose |
|------------|---------|
| **Docker** | Containerisation |
| **Nginx** | Web server |
| **Docker Compose** | Multi-container management |
| **Docker Hub** | Image registry |
| **GitHub Actions** | CI/CD pipeline |
| **AWS ECS** | Container deployment |
| **Kubernetes** | Container orchestration |
| **AWS EKS** | Managed Kubernetes |

---

## 📁 Project Structure
```
docker-app/
├── Dockerfile           # Docker image definition
├── index.html           # Web application
├── docker-compose.yml   # Multi-container setup
├── deployment.yaml      # Kubernetes deployment
├── .gitignore           # Git ignore file
└── .github/
    └── workflows/
        └── deploy.yml   # CI/CD pipeline
```

---

## ⚙️ Prerequisites

- Docker installed
- Docker Hub account
- AWS CLI configured
- kubectl installed (for Kubernetes)

---

## 🚀 How to Run Locally

**1. Clone the repository:**
```bash
git clone https://github.com/vames1/docker-app.git
cd docker-app
```

**2. Build the Docker image:**
```bash
docker build -t my-web-app .
```

**3. Run the container:**
```bash
docker run -d -p 8080:80 my-web-app
```

**4. Visit in browser:**
```
http://localhost:8080
```

---

## 🐙 Docker Compose

**Start all services:**
```bash
docker-compose up -d
```

**Stop all services:**
```bash
docker-compose down
```

---

## ⚙️ Kubernetes Deployment

**Deploy to Kubernetes:**
```bash
kubectl apply -f deployment.yaml
```

**Check pods:**
```bash
kubectl get pods
```

**Get service URL:**
```bash
kubectl get services
```

---

## 🔄 CI/CD Pipeline

Every push to `master` branch automatically:
1. ✅ Builds Docker image
2. ✅ Pushes to Docker Hub
3. ✅ Deploys to AWS ECS

---

## 🌍 Key Features

- ✅ Custom Nginx web application
- ✅ Docker Networking with custom bridge network
- ✅ Docker Volumes for persistent data
- ✅ Docker Compose for multi-container apps
- ✅ Automated CI/CD with GitHub Actions
- ✅ Kubernetes deployment on AWS EKS
- ✅ Zero downtime deployments

---

## 👨‍💻 Author

**Victor Oluwaseyi Akindiose**
Cloud Engineer | Lagos, Nigeria
- 🌍 Portfolio: https://vames1.github.io
- 📧 Email: victoroluwaseyi2018@gmail.com
- 🐙 GitHub: https://github.com/vames1
