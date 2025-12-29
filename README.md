Hello Node.js – Dockerized REST API

This project is a simple Node.js + Express REST API that returns a Hello World! response.
The application is Dockerized and deployed on an AWS EC2 instance as part of a DevOps assignment.

📌 Project Overview

Simple REST API using Node.js & Express

Runs on port 3000

Fully Dockerized

Deployed and tested on AWS EC2

Optional Docker Compose support

🛠 Tech Stack

Node.js

Express.js

Docker

AWS EC2

Git & GitHub

📂 Project Structure
hello-node/
├── Dockerfile
├── docker-compose.yml
├── main.js
├── package.json
├── package-lock.json
└── README.md

🚀 API Details
Endpoint
GET /

Response
Hello World!

▶️ Run Application Locally (Without Docker)
1. Install dependencies
npm install

2. Start the server
node main.js

3. Access the API
http://localhost:3000

🐳 Run Application Using Docker
1. Build Docker Image
docker build -t hello-node-app .

2. Run Docker Container
docker run -d -p 3000:3000 --name hello-node-container hello-node-app

3. Access the API
http://localhost:3000

🧩 Run Using Docker Compose (Bonus)
1. Start services
docker-compose up -d

2. Access the API
http://localhost:3000

☁️ Deployment on AWS EC2

Steps followed:

Launched EC2 instance (Amazon Linux)

Installed Docker and Git

Cloned this repository

Built Docker image

Ran container exposing port 3000

Opened port 3000 in EC2 Security Group

Public Access
http://<EC2_PUBLIC_IP>:3000

🔐 EC2 Security Group Configuration

Inbound rule added:

Port: 3000

Protocol: TCP

Source: 0.0.0.0/0

📌 Key Learnings

Dockerizing a Node.js application

Running containers on EC2

Port exposure and networking

GitHub version control

Basic DevOps workflow
