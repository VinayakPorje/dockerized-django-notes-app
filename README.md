# 🐳 Dockerized Django Notes App

## 📌 Overview

This project demonstrates a production-style **multi-container Docker deployment** of a Django Notes Application using:

- Nginx (Reverse Proxy)
- Django 
- MySQL (Database)
- Docker Compose
- AWS EC2

This repository focuses on Docker architecture, container networking, and cloud deployment.

---

## 🏗️ Architecture

Client → Nginx (Port 80 - Public) → Django (Port 8000 - Internal) → MySQL (Port 3306 - Internal)

- Only Port 80 is publicly accessible.
- Django runs internally on port 8000.
- MySQL runs internally on port 3306.
- All containers communicate via a custom Docker network.

---

## 🧱 Services & Ports

| Service | Role | Port |
|----------|------|------|
| Nginx | Reverse Proxy | 80 |
| Django | Application Server | 8000 |
| MySQL | Database | 3306 |

---

## 🚀 How to Run

1. Install Docker and Docker Compose
2. Clone the repository
3. Run:

```bash
docker-compose up --build -d
```

4. Access the app:

http://<EC2_PUBLIC_IP>

---

## 🧠 DevOps Concepts Demonstrated

- Multi-container Docker setup
- Reverse proxy configuration using Nginx
- Docker networking between services
- Persistent database storage using volumes
- Cloud deployment on AWS EC2 (Linux)

---

## 📦 Tech Stack

- Python
- Django
- MySQL
- Nginx
- Docker
- Docker Compose
- AWS EC2

---

## 👨‍💻 Author

Vinayak Porje  
DevOps | Cloud 
