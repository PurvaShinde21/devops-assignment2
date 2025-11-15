# 🚀 DevOps Assignment 2

This project demonstrates how to create a simple Flask application, containerize it using Docker, push the code to GitHub, and upload the Docker image to Docker Hub.

---

## 📁 Project Structure

```
devops-assignment2/
├── app.py
├── requirements.txt
├── Dockerfile
└── README.md
```

---

## 📝 Steps Performed

### 1️⃣ Create Flask Application

A simple Flask app was created that returns a welcome message on `/`.

### 2️⃣ Create Dockerfile

The Dockerfile includes:
- Python base image  
- Installing dependencies  
- Copying project files  
- Exposing port 5000  
- Running the Flask application  

### 3️⃣ Build Docker Image

```bash
docker build -t flask-demo:latest .
```

### 4️⃣ Test Docker Image Locally

```bash
docker run --rm -p 5000:5000 flask-demo:latest
```

### 5️⃣ Tag Image for Docker Hub

```bash
docker tag flask-demo:latest purvashinde21/flask-demo:latest
```

### 6️⃣ Push Image to Docker Hub

```bash
docker push purvashinde21/flask-demo:latest
```

### 7️⃣ Push Code to GitHub

```bash
git add .
git commit -m "Added Flask app, Dockerfile, and project setup"
git push origin main
```

---

## 🔗 Links

### ✔ GitHub Repository  
👉 https://github.com/PurvaShinde21/devops-assignment2

### ✔ Docker Hub Image  
👉 https://hub.docker.com/r/purvashinde21/flask-demo

---

## 👩‍💻 Author
**Purva Shinde**



