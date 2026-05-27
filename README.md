# Software Engineering in Practice — Assignment 1 (2026)
## Prerequisites
- Git
- Docker Desktop
- Minikube
- kubectl
## Setup
### 1. Clone the repository
```bash
git clone https://github.com/StefaniaKoulouri/seip_assignment_1_2026.git
cd seip_assignment_1_2026
```
### 2. Start Minikube
```bash
minikube start --driver=docker
```
### 3. Apply Kubernetes manifests
```bash
kubectl apply -f k8s/
```
### 4. Port forward
```bash
kubectl port-forward service/echo-api-service 8080:80
```
### 5. Test the endpoints
- http://localhost:8080/
- http://localhost:8080/secure-config
