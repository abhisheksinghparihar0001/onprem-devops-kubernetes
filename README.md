# onprem-devops-kubernetes
Tier-3 DevOps project deployed on on-premise infrastructure using Docker, Kubernetes (Minikube), Nginx, and HPA.

# Tier-3 DevOps Project (On-Premise)

This project demonstrates a complete **Tier-3 application architecture** deployed on **on-premise infrastructure** using modern DevOps tools and practices.

---

## 🚀 Tech Stack
- **Frontend:** HTML + Nginx
- **Backend:** Node.js (Express)
- **Containerization:** Docker
- **Orchestration:** Kubernetes (Minikube)
- **Reverse Proxy:** Nginx
- **Auto Scaling:** Horizontal Pod Autoscaler (HPA)
- **Infrastructure:** On-Premise Ubuntu Server

---

## 🏗 Architecture Overview
- Frontend and Backend are containerized using Docker
- Deployed on Kubernetes (Minikube)
- Nginx acts as a reverse proxy
- Services expose applications internally
- HPA automatically scales pods based on CPU utilization

---

tier3-devops-project/
│
├── frontend/
│   ├── Dockerfile          # Frontend container build file
│   └── index.html          # Static frontend page
│
├── backend/
│   ├── Dockerfile          # Backend container build file
│   └── app.js              # Node.js API
│
├── nginx/
│   └── nginx.conf          # Reverse proxy config
│
├── k8s/
│   ├── frontend-deploy.yaml  # Frontend deployment
│   ├── backend-deploy.yaml   # Backend deployment
│   ├── frontend-hpa.yaml     # Frontend auto-scaling
│   ├── backend-hpa.yaml      # Backend auto-scaling
│   └── services.yaml         # Services for frontend & backend
