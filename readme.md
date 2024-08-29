# FastAPI Dockerized Project

## Overview

This project demonstrates how to:
1. Create a FastAPI application.
2. Containerize the application using Docker.
3. Manage Docker containers.
4. Set up a private Docker registry.
5. Push images to Docker Hub.

## Prerequisites

- Docker installed on your machine.
- Docker Compose (optional, for multi-container setups).
- Basic understanding of Docker and FastAPI.

## Setup and Deployment

### 1. Install Docker and Docker Compose

**On Ubuntu (via WSL2):**
### 3. Create virtual enviroment and activate it then run further commands

** Install venv for Linux:- sudo apt-get install python3-venv**
**Create virtual environment:- py -m venv venv**
**Activate virtual env for Linux:- source venv/bin/activate**
**Activate virtual env for Windows:- .\venv\Scripts\activate**

### 2. Use this command to verify the installation by running test container
**docker run hello-world**

###3. Use this command to build the docker image from Dockerfile
**docker build -t fastapi-app .**

###4. Run the docker container form image
**docker run -d -p 80:80 fastapi-app**
**access the webapp by entering this "localhost:80/docs" to browser**

###5. To start, stop, remove and list containers
**docker start <container_id>**
**docker stop <container_id>**
**docker rm <container_id>**
**docker ps**

###6. Dokcer compose command to create image
**docker run -d -p 80:80 fastapi-app**
**access the webapp by entering this "localhost:80/docs" to browser**

###7.Push an image to private registry
**docker login**
**docker tag fastapi-app localhost:8000/fastapi-app:latest**
**docker push localhost:8000/fastapi-app:latest**
