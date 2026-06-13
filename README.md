# Docker Compose Multi-Container Application

## Project Overview

This project demonstrates how to use Docker Compose to manage multiple containers in a single application.

The application consists of:

- Flask Web Application
- MySQL Database Container
- Docker Compose Configuration
- Docker Networking
- Docker Volumes

The Flask application runs inside a Docker container and is managed using Docker Compose.

---

## Project Architecture

```text
Browser
   ↓
Flask Container
   ↓
MySQL Container
```

---

## Technologies Used

- Python
- Flask
- Docker
- Docker Compose
- MySQL
- Git
- GitHub

---

## Project Structure

```text
docker-compose-project/
│
├── app.py
├── requirements.txt
├── Dockerfile
└── docker-compose.yml
```

---

## Features

- Containerized Flask Application
- Multi-Container Deployment
- Docker Compose Automation
- Docker Networking
- Persistent Storage using Docker Volumes
- Easy Container Management

---

## How to Run

### Build and Start Containers

```bash
docker compose up -d
```

### Verify Running Containers

```bash
docker compose ps
```

### Stop Containers

```bash
docker compose down
```

---

## Output

Open:

```text
http://localhost:5000
```

Output:

```text
Docker Compose Project Running Successfully!
```

---

## Challenges Faced and Solutions

### 1. Undefined Volume Error

Error:

```text
service "mysql" refers to undefined volume mysql_data
```

Cause:

Volume name mismatch between service configuration and volume definition.

Solution:

Ensured the volume name was consistent throughout the docker-compose.yml file.

---

### 2. Docker Compose Configuration Issues

Cause:

Incorrect YAML formatting and naming inconsistencies.

Solution:

Corrected Docker Compose syntax and verified proper indentation.

---

### 3. Port Conflict Issue

Error:

```text
Bind for 0.0.0.0:3306 failed
```

Cause:

Port 3306 was already being used on the host machine.

Solution:

Identified the port conflict and updated port mappings accordingly.

---

### 4. Container Startup Troubleshooting

Issue:

MySQL container remained in Created state.

Solution:

Used Docker commands such as:

```bash
docker ps -a
docker logs
docker inspect
```

to diagnose and troubleshoot container startup problems.

---

## Learning Outcomes

Through this project I learned:

- Docker Compose Fundamentals
- Multi-Container Application Management
- Docker Networking
- Docker Volumes
- Container Lifecycle Management
- Port Mapping
- Debugging Docker Containers
- YAML Configuration
- DevOps Troubleshooting Techniques

---

## Future Improvements

- Connect Flask Application with MySQL Database
- Add CRUD Operations
- Implement User Authentication
- Deploy on AWS EC2
- Integrate CI/CD Pipeline using Jenkins

---

## Author

**Revunuru Sarada Maheswari**

B.Tech Computer Science and Engineering

DevOps & Cloud Computing Aspirant
