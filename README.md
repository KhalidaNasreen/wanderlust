# Wanderlust

Wanderlust is a full-stack web application deployed on AWS EC2 using Docker and Jenkins.

## Project Overview

The application is containerized using Docker and deployed through a Jenkins CI/CD pipeline. The source code is maintained on GitHub, and Jenkins handles the build and deployment process.

## Tech Stack

* AWS EC2
* Jenkins
* Docker
* Docker Compose
* Git
* GitHub
* Node.js
* React
* MongoDB
* Redis

## CI/CD Pipeline

```text
GitHub
   ↓
Jenkins
   ↓
Checkout
   ↓
Test
   ↓
Build Docker Images
   ↓
Deploy
   ↓
Verify
```

## Jenkins Pipeline

The Jenkins pipeline consists of the following stages:

* Checkout – pulls the latest code from GitHub
* Test – installs backend dependencies
* Build – builds the Docker images
* Deploy – starts the application using Docker Compose
* Verify – checks the deployed containers

## Docker

The application runs using Docker Compose with the following services:

* Frontend
* Backend
* MongoDB
* Redis

## Deployment

The application is deployed on an Ubuntu EC2 instance on AWS.

Jenkins automatically pulls the latest code, builds the Docker images, and deploys the application using Docker Compose.

## CI/CD Screenshot

Add the Jenkins Pipeline Stage View screenshot here.

## Author

Khalida Nasreen
