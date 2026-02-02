# Kubernetes-Deployment-with-Minikube

Prerequisites

Ensure the following tools are installed:

* Docker
* kubectl
* Minikube
* Git

Verify installations:

```bash
docker --version
kubectl version --client
minikube version
```

---

## 📁 Project Structure

```
.
├── app/
│   ├── index.js
│   ├── package.json
│   └── Dockerfile
├── k8s/
│   ├── deployment.yaml
│   └── service.yaml
└── README.md
```

---

Step 1: Start Minikube

```bash
minikube start
```
---
Step 2: Deploy to Kubernetes

```bash
kubectl apply -f k8s/
```

Verify resources:

```bash
kubectl get deployments
kubectl get pods
kubectl get svc
```

---

Step 3: Access the Application

Use Minikube to expose the service:

```bash
minikube service demo-service
```

This opens the application in the browser.

Expected output:

```
Hello from Kubernetes 🚀
```




