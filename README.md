# 🌍 Dockerized NGINX Hello World

A simple project to demonstrate how to serve a static "Hello, World" webpage using **NGINX** in a custom **Docker** container. This project is ideal for learning containerization fundamentals and basic web server configuration.

---

## 📌 Project Overview

* **Name**: docker-nginx-hello-world
* **Stack**: Docker, NGINX, HTML
* **Goal**: Serve a static "Hello, World" page using a lightweight container
* **Use Case**: Introductory DevOps project for Docker and web server deployment basics

---

## 📁 Project Structure

```
├── Dockerfile         # Custom image that serves a static HTML page using NGINX
├── index.html         # (Assumed) Static HTML file with "Hello, World" message
```

> Note: If `index.html` is baked into the image, ensure it's copied during the Docker build.

---

## 🚀 Getting Started

### Prerequisites

* [Docker](https://www.docker.com/products/docker-desktop)

### Installation Steps

```bash
# 1. Clone the repository
git clone https://github.com/davidhernandez-adm/docker-nginx-hello-world.git
cd docker-nginx-hello-world

# 2. Build the Docker image
docker build -t nginx-hello .

# 3. Run the container
docker run -p 8080:80 nginx-hello

# 4. Access the page
open http://localhost:8080
```

---

## 📦 Technologies Used

* **Docker** – Containerization platform
* **NGINX** – Static content web server
* **HTML** – Frontend display ("Hello, World")

---

## 🧪 Testing and Coverage

> Test by accessing `http://localhost:8080`. You should see a "Hello, World" page.

---

## 🧠 Key Challenges & Learnings

* Learned how to create a custom Dockerfile for a static web server
* Understood NGINX default directory structure for serving content
* Practiced image building, port mapping, and container lifecycle

---

## 📷 Screenshots or Live Demo

> Screenshot of browser with `Hello, World` page can be added here

---

## 📜 License

[MIT](https://opensource.org/licenses/MIT)

---

> Created by [David Hernández](https://github.com/davidhernandez-adm) as a foundational exercise in Docker and web server deployment.
