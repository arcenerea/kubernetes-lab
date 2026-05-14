# ☸️ Kubernetes Lab

Hands-on Kubernetes lab using Minikube — cluster setup, application deployment, service exposure, and live traffic validation.

Built and documented by [Nerea Arce](https://www.linkedin.com/in/nerea-arce/)  
Platform Engineer | DevOps | SysAdmin

---

## 📌 What this project covers

This lab demonstrates a complete local Kubernetes workflow using Minikube.

It includes:

- Local Kubernetes cluster setup
- Application deployment using Deployment manifests
- Service exposure using NodePort
- Live HTTP traffic validation inside the cluster
- Basic debugging and cluster inspection using kubectl

---

## 🏗️ Architecture

```text
User
  ↓
NodePort Service (hello-app)
  ↓
Kubernetes Deployment
  ↓
Pod (hello-app container)
