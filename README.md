# ☸️ Kubernetes Lab

Hands-on Kubernetes lab using Minikube — cluster setup, app deployment, service exposure and live traffic.

Built and documented by [Nerea Arce](https://www.linkedin.com/in/nerea-arce/) · Platform Engineer · DevOps

---

## What this lab covers

- Local Kubernetes cluster with Minikube
- App deployment using Kubernetes Deployment manifest
- Service exposure with NodePort
- Live HTTP traffic served from inside the cluster

---

## Cluster running

![Kubernetes cluster](cluster.jpg)

---

## App responding

![App running](app-running.jpg)

---

## Files

| File | Description |
|------|-------------|
| `deployment.yaml` | Kubernetes Deployment — hello-app with 1 replica |
| `service.yaml` | NodePort Service — exposes app on port 8080 |

---

## How to run

Start the cluster:

    minikube start --driver=docker

Apply the manifests:

    kubectl apply -f deployment.yaml
    kubectl apply -f service.yaml

Check everything is running:

    kubectl get pods,deployments,services

Get the app URL:

    minikube service hello-app --url

Test the app:

    curl <url>

---

## Output

    Hello, world!
    Version: 1.0.0
    Hostname: hello-app-66cdc8598f-sch8c

---

## Tech stack
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

---

## Author
**Nerea Arce** — SysAdmin · DevOps · Cloud Infrastructure
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/nerea-arce/)
[![GitHub](https://img.shields.io/badge/GitHub-arcenerea-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/arcenerea)
