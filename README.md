# DevOps CI/CD Pipeline Project

## Overview
This project demonstrates a CI/CD pipeline built using Jenkins and Podman.

## Architecture

---
        ┌───────────────┐
        │   Developer   │
        └───────┬───────┘
                │ git push
                ▼
        ┌───────────────┐
        │     GitHub    │
        │   Repository  │
        └───────┬───────┘
                │ trigger
                ▼
        ┌───────────────┐
        │    Jenkins    │
        │   CI/CD Job   │
        └───────┬───────┘
                │
        ┌───────▼────────┐
        │ Clone Source    │
        │ Build Image     │
        │ Run Container   │
        └───────┬────────┘
                │
                ▼
        ┌───────────────┐
        │  Podman       │
        │ Container     │
        └───────┬───────┘
                │
                ▼
        ┌───────────────┐
        │  Web App      │
        │ localhost:8081│
        └───────────────┘


## Tools Used
- Jenkins
- Podman
- GitHub
- Linux
- Nginx

## Project Structure

```
devops-cicd-project
│
├── app/
│   ├── index.html
│   └── style.css
│
├── Dockerfile/Containerfile
│
├── Jenkinsfile
│
├── screenshots/
│   ├── jenkins-pipeline.png
│   ├── console-output.png
│   └── deployed-app.png
│
└── README.md
```
## Application
Accessible at:
http://localhost:8081


# Project Screenshots 📸

### Jenkins Dashboard
![Jenkins Dashboard](screenshots/jenkins-dashboard.png)

---

### Jenkins Pipeline Success
![Pipeline Success](screenshots/jenkins-pipeline-success.png)

---

### Jenkins User Profile
![User Profile](screenshots/jenkins-user-profile.png)

---

### Application Deployment
![Application Deployment](screenshots/app-deployment-success.png)

---








