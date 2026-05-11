# Production Grade Kubernetes Platform

A production-oriented cloud-native web platform showcasing containerization, Kubernetes orchestration, autoscaling, deployment strategies, ingress routing, and scalable microservice deployment practices.

---

# Project Overview

This project demonstrates end-to-end deployment of a full-stack application using:

- Docker
- Docker Compose
- Kubernetes
- Horizontal Pod Autoscaler (HPA)
- Canary Deployment
- Blue-Green Deployment
- Rolling Updates
- Kubernetes Services
- Ingress Controller
- ConfigMaps
- Secrets
- Namespace Isolation

---

# Tech Stack

## Containerization
- Docker
- Docker Compose

## Orchestration
- Kubernetes
- Minikube

## Kubernetes Components
- Deployments
- Services
- Ingress
- ConfigMaps
- Secrets
- HPA

## Deployment Strategies
- Rolling Update
- Blue-Green Deployment
- Canary Deployment

---

# Repository Structure

backend/
frontend/

k8_manifests/
 ├── blue-green/
 ├── canary/
 ├── rollingUpdate/
 ├── ingress/
 ├── secrets/
 └── config_map/

docker-compose.yml


# Features
- Containerized frontend and backend services
- Kubernetes-native application deployment
- Service-to-service communication
- Ingress-based routing
- Horizontal autoscaling using Metrics Server + HPA
- Canary deployment implementation
- Blue-Green deployment strategy
- Rolling update strategy
- Namespace isolation
- Config and secret management
- Scalable infrastructure design

# Autoscaling
- Horizontal Pod Autoscaler (HPA) configured for:
- Frontend deployments
- Backend deployments
Metrics used:
- CPU Utilization
- Memory Utilization
HPA dynamically scales pods based on resource consumption to improve scalability and availability.

# Deployment Strategies Implemented
- Rolling Updates
    Gradual replacement of old pods with updated pods without downtime.
- Blue-Green Deployment
    Two identical production environments with controlled traffic switching for safer releases.
- Canary Deployment
    Controlled traffic shifting to validate new application versions before full rollout.

# Local Setup
- Clone Repository
    git clone <repo-url>
    cd production-grade-k8s-platform
  
- Run Using Docker Compose
    docker compose up -d


- Kubernetes Deployment
    Start Minikube
      Bash: minikube start

    Enable Ingress
      Bash: minikube addons enable ingress

    Apply Kubernetes Manifests
      Bash: kubectl apply -f k8_manifests/

    Verify Kubernetes Resources
      Bash
       kubectl get pods
       kubectl get svc
       kubectl get ingress
       kubectl get hpa

# Kubernetes Concepts Implemented
       Pods
       Deployments
       ReplicaSets
       Services
       Ingress Controllers
       Namespaces
       ConfigMaps
       Secrets  
       HPA
       Resource Requests & Limits
       Deployment Strategies

# Author
Harsh Verma
DevOps | Kubernetes | Docker | Cloud-Native Engineering 
