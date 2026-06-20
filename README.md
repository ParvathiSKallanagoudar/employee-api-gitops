# Employee API GitOps Deployment using ArgoCD

## Project Overview

This project demonstrates the implementation of GitOps Continuous Delivery using ArgoCD on Kubernetes.

The project deploys a Spring Boot Employee API application using Kubernetes manifests stored in GitHub. ArgoCD continuously monitors the repository and ensures that the Kubernetes cluster state always matches the desired state defined in Git.

The project also demonstrates Auto Sync, Self-Healing, Configuration Drift Detection, and Git-based Rollback strategies.

---

## Technologies Used

* ArgoCD
* Kubernetes
* Docker
* GitHub
* Jenkins
* Prometheus
* Grafana
* Linux
* Spring Boot

---

## Architecture

<img width="1024" height="559" alt="image" src="https://github.com/user-attachments/assets/46043eb2-5ad6-4e1c-9b9c-2029a5ebd704" />

---

## Features Implemented

* ArgoCD Installation on Kubernetes
* GitOps Deployment Model
* GitHub Repository Integration
* Kubernetes Manifest Management
* Auto Sync Configuration
* Self-Healing Configuration
* Configuration Drift Detection
* Manual Synchronization
* Git-Based Rollback
* Application Monitoring with Prometheus and Grafana

---

## GitOps Workflow

1. Developer updates Kubernetes manifests in GitHub.
2. ArgoCD detects the new commit.
3. ArgoCD compares desired state and actual state.
4. ArgoCD synchronizes Kubernetes resources automatically.
5. Kubernetes cluster is updated without manual deployment commands.

---

## ArgoCD Application Dashboard

<img width="1907" height="867" alt="Screenshot 2026-06-20 184133" src="https://github.com/user-attachments/assets/8f245879-7e25-4f58-8483-55611a7c75cc" />


### ArgoCD Features Demonstrated

- GitOps Continuous Delivery
- Automated Synchronization
- Self-Healing
- Configuration Drift Detection
- Desired State vs Actual State Management
- Git-Based Rollback

The dashboard shows the Employee API application in a Healthy and Synced state, with Kubernetes Deployment, Service, ReplicaSets, and Pods managed through ArgoCD.
---
## Configuration Drift Demonstration

A manual scaling operation was performed using:

kubectl scale deployment employee-api --replicas=5

ArgoCD detected the drift and automatically restored the deployment to the desired state defined in Git.

---

## Monitoring and Observability

Prometheus was configured to scrape Spring Boot Actuator metrics exposed by the Employee API application.

Grafana dashboards were created to visualize application health and performance metrics including:

- Live JVM Threads
- HTTP Request Count
- CPU Usage
- JVM Memory Usage

### Grafana Dashboard
<img width="1920" height="861" alt="Grafana Monitoring Dashboard-1" src="https://github.com/user-attachments/assets/0d25e316-35f3-4b7a-9012-e3cbc98c1203" />


### JVM and Resource Monitoring

<img width="1920" height="866" alt="Grafana Monitoring Dashboard-2" src="https://github.com/user-attachments/assets/267e87ef-d01c-4bf6-a81c-a2d0453acc90" />


---

## Learning Outcomes

* Understanding GitOps Principles
* Desired State vs Actual State
* ArgoCD Architecture
* Kubernetes Resource Synchronization
* Auto Sync and Self-Healing
* Git-Based Deployment Management
* Production-Style Continuous Delivery

---

## Author

Parvathi S Kallanagoudar
DevOps Engineer (Fresher)
