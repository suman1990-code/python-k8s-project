# python-k8s-project
# Python Kubernetes Deployment Project

This project demonstrates deploying a Dockerized Python application on Kubernetes with features like self-healing and auto-scaling.

## 📁 Project Structure
- app.py – Python application
- requirements.txt – Dependencies
- deployment.yaml – Kubernetes Deployment configuration
- service.yaml – Kubernetes Service configuration

## 🚀 Deployment Steps

1. Build Docker image:
   docker build -t python-k8s-app .

2. Push image to Docker Hub:
   docker push <your-dockerhub-username>/python-k8s-app

3. Apply Kubernetes manifests:
   kubectl apply -f deployment.yaml
   kubectl apply -f service.yaml

4. Verify:
   kubectl get pods
   kubectl get services

5. Access application:
   minikube service <service-name>

## ⚙️ Features
- Containerized using Docker
- Kubernetes Deployment & Service
- Self-healing (auto pod restart)
- Scalable using HPA

