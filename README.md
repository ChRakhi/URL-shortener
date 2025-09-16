# 🚀 URL Shortener Service

A **scalable, containerized URL shortener** that allows users to submit long URLs and receive shortened versions. Built with **Python (Flask)**, this service leverages **Redis** for fast in-memory storage and is fully deployable on **Docker** and **Kubernetes**, featuring **load balancing**, **auto-scaling**, and **secure configuration management**.  

---

## 🛠 Tech Stack

- **Backend:** Python (Flask)  
- **Database:** Redis (in-memory key-value store)  
- **Containerization:** Docker  
- **Orchestration:** Kubernetes  
- **Networking:** Kubernetes Services (ClusterIP, LoadBalancer)  
- **Configuration Management:** ConfigMaps & Secrets  
- **Scaling:** Horizontal Pod Autoscaler (HPA)  

---

## 📦 Features

- Shorten long URLs and retrieve them using a unique short code  
- Fast, in-memory storage using Redis  
- Fully containerized with Docker for consistent deployment  
- Kubernetes deployment with replicas for **high availability**  
- Load balancing across multiple application instances  
- Auto-scaling based on traffic using HPA  
- Secure configuration management using ConfigMaps & Secrets  

---

## 📈 Architecture Overview

```text
User Request
      │
      ▼
Kubernetes LoadBalancer
      │
      ▼
Flask Application Pods
      │
      ▼
     Redis
      │
      ▼
ConfigMaps & Secrets for secure configuration
      │
      ▼
Horizontal Pod Autoscaler (HPA) for scaling
