# ITI Docker & DevOps Labs 🐳

![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
![Nginx](https://img.shields.io/badge/nginx-%23009639.svg?style=for-the-badge&logo=nginx&logoColor=white)
![Flask](https://img.shields.io/badge/flask-%23000.svg?style=for-the-badge&logo=flask&logoColor=white)
![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=for-the-badge&logo=mysql&logoColor=white)
![WordPress](https://img.shields.io/badge/wordpress-%2321759b.svg?style=for-the-badge&logo=wordpress&logoColor=white)

This repository contains my solutions for Docker labs during the ITI training program. Each lab focuses on different aspects of containerization, networking, and orchestration.

## Labs Overview

### [Lab 1: Docker Basics & Cgroups](./Lab1/README.md)
* Resource limits (CPU/Memory).
* Running Nginx and Apache containers.
* Deep dive into Linux Control Groups (cgroups) to inspect system-level resource constraints.

### [Lab 2: Custom Images & Networking](./Lab2/README.md)
* Dockerizing a Python Flask application.
* Creating custom bridge networks with specific subnets (`10.0.0.0/8`).
* Using Docker Volumes for persistent static HTML content.

### [Lab 3: Registry & Orchestration](./Lab3/README.md)
* Setting up an insecure local Private Docker Registry.
* Multi-container orchestration using **Docker Compose**.
* Deploying WordPress with a MySQL backend.
* **Bonus:** Deploying a multi-tier application using Nginx as a reverse proxy for the Flask app.

## Key Highlights & Troubleshooting
Throughout these labs, I tackled real-world deployment challenges, including:
* **Debugging Build Failures:** Upgraded base images (e.g., Python 3.6 to 3.13) to resolve outdated package metadata and dependency issues.
* **Port Conflict Resolution:** Investigated and resolved host port conflicts (e.g., identifying Oracle TNS Listener on port 8080 via `netstat` and stopping the service) to ensure seamless container mapping.
* **Reverse Proxy Setup:** Successfully routed traffic using an Nginx reverse proxy configuration (`proxy_pass`) to a backend Flask service.

---
**Author:** Mohamed Nada  
**Tech Stack:** Docker, Docker Compose, Nginx, Flask, MySQL, Linux/WSL.
