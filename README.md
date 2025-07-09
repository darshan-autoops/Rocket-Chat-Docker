# 🚀 Rocket.Chat Docker Deployment

This project demonstrates how to deploy Rocket.Chat using Docker Compose and MongoDB (replica set).

## 📦 Prerequisites

- Docker
- Docker Compose

## 🛠️ Setup Instructions

1. **Clone the Repository**

```bash
git clone https://github.com/yourusername/rocketchat-docker-deployment.git
cd rocketchat-docker-deployment

-docker-compose up -d

docker exec -it <mongo-container-name> /bin/bash

mongosh
---------------------------------------------------------------------------
docker run -d --name db -p 27017:27017 mongo:latest
docker run -d --name rocketchat -p 3000:3000 --link db:db rocket.chat



