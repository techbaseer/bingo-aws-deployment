# Bingo Application – End-to-End DevOps Project

## Overview
This repository represents a complete DevOps lifecycle project built
around a real-time Bingo application. The goal of this project is to
design, deploy, secure, and operate an application using modern
DevOps and cloud-native tools, following real industry practices.

The project covers infrastructure provisioning, containerization,
CI/CD pipelines, orchestration, monitoring, and security, implemented
incrementally within the same repository.

## Application Background
The Bingo application is an open-source real-time multiplayer game
built using Next.js, React, and Socket.io (WebSockets).

The application logic is open-source and is used here as a base to
demonstrate DevOps, DevSecOps, and cloud deployment practices.

## DevOps Stack Used

Version Control:
- Git
- GitHub

Cloud & Infrastructure:
- AWS EC2
- Ubuntu Linux
- AWS Security Groups

Web & Runtime:
- Node.js
- Nginx (Reverse Proxy)
- PM2 (Process Manager)

Containerization:
- Docker
- Docker Compose

CI/CD:
- Jenkins

Orchestration:
- Kubernetes (EKS)

Monitoring & Observability:
- Prometheus
- Grafana

Security:
- OWASP best practices
- Trivy vulnerability scanning

## Project Phases

Phase 1: EC2-Based Deployment
- Application deployed on AWS EC2
- Node.js environment configured as per engine requirements
- Application exposed via Nginx reverse proxy (80 → 3000)
- PM2 used for process management
- Real-world production issues resolved (networking, ports, gateway errors)

Phase 2: Containerization
- Dockerfile created for the application
- Docker images built and executed
- Docker Compose used for multi-service management

Phase 3: CI/CD Pipeline
- Jenkins pipeline implemented
- Automated build and deployment workflows
- Integration with GitHub repository

Phase 4: Kubernetes Orchestration
- Application deployed on Kubernetes (EKS)
- Kubernetes manifests used for deployments and services
- Scalability and rolling updates handled via Kubernetes

Phase 5: Monitoring & Security
- Prometheus configured for metrics collection
- Grafana dashboards for visualization
- Trivy used for container vulnerability scanning
- Security best practices applied throughout the pipeline

## Architecture Overview

User
 ↓
Browser
 ↓
Nginx
 ↓
Application (Next.js / Socket.io)
 ↓
Container Runtime
 ↓
Kubernetes Cluster

## How to Run (Development / Server)

npm install
npm run dev

Or run in background:

nohup npm run dev &

## Learning Objectives
- End-to-end DevOps workflows
- Practice real-world production deployments
- CI/CD automation with Jenkins
- Work with Docker and Kubernetes
- Apply monitoring and security in DevOps pipelines
- Gain hands-on cloud troubleshooting experience

## Notes
This repository is intentionally designed as a single evolving DevOps
project, where all tools and stages are implemented progressively.
The focus is on learning, experimentation, and real-world simulation
of enterprise DevOps environments.
