# React-Vite-Jenkins-SonarQube-Docker-DockerSwarm-CI-CD-Pipeline
CI/CD Pipeline for React Vite Application using Jenkins, SonarQube, Docker &amp; Docker Swarm
---
## Project Overview

This project demonstrates a complete DevOps CI/CD pipeline for deploying a React Vite frontend application using Jenkins, Node.js, SonarQube, Docker, and Docker Swarm.

The pipeline automates the process of installing dependencies, building the application, analyzing code quality, containerizing, and deploying the application.

---

## Tools & Technologies

- Jenkins  
- Node.js / npm  
- SonarQube  
- Docker  
- Docker Hub  
- Docker Swarm  
- GitHub  
- Nginx  

---

## Architecture

Developer pushes code to GitHub → Jenkins triggers pipeline → npm installs dependencies → Vite builds production files → SonarQube performs code analysis → Quality Gate validation → Docker image build (Nginx) → Push image to DockerHub → Deploy container using Docker Swarm.

---

## Pipeline Workflow

1. Pull source code from GitHub repository.  
2. Install project dependencies using npm.  
3. Build production-ready files using Vite (`dist/` folder).  
4. Perform code quality and security analysis using SonarQube.  
5. Validate code using SonarQube Quality Gate.  
6. Build Docker image using Nginx to serve static files.  
7. Push Docker image to DockerHub.  
8. Deploy application using Docker Swarm.  

---

## Jenkins Pipeline Stages

- Clone Repository  
- Install Dependencies  
- Build Production Files  
- SonarQube Analysis  
- Quality Gate  
- Docker Build  
- Push Docker Image  
- Deploy to Docker Swarm  

---

## Docker Deployment

The application is containerized using Docker with Nginx as the web server and deployed across nodes using Docker Swarm.

The deployment uses a `docker-compose.yml` file with multiple replicas for scalability and load distribution.

## Project Structure
