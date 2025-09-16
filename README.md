🚀 URL Shortener Service

A scalable, containerized URL shortener that allows users to submit long URLs and receive shortened versions. Built with Python (Flask), this service leverages Redis for fast in-memory storage and is fully deployable on Docker and Kubernetes, with load balancing, auto-scaling, and secure configuration management.

🛠 Tech Stack

Backend: Python (Flask)

Database: Redis (in-memory key-value store)

Containerization: Docker

Orchestration: Kubernetes

Networking: Kubernetes Services (ClusterIP, LoadBalancer)

Configuration Management: ConfigMaps & Secrets

Scaling: Horizontal Pod Autoscaler (HPA)

📦 Features

Shorten long URLs and retrieve them using a short code

Fast, in-memory storage using Redis

Containerized with Docker for easy deployment

Deployable on Kubernetes with replicas for high availability

Load balancing across multiple instances

Auto-scaling based on traffic using HPA

Secure configuration management with ConfigMaps and Secrets

📈 Architecture Overview

User Request → Sent to Kubernetes LoadBalancer

Flask Application Pods → Handle URL shortening & retrieval

Redis Container → Stores URL mappings in-memory

HPA → Scales pods automatically based on CPU usage

ConfigMaps & Secrets → Securely manage configuration

🔑 Key Learnings

Containerized a Python microservice using Docker

Deployed a multi-container application on Kubernetes

Implemented ConfigMaps & Secrets for secure configuration

Configured load balancing and auto-scaling with HPA

Gained practical experience in microservice architecture, orchestration, and monitoring
