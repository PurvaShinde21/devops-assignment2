# DevOps Assignment 2

This assignment demonstrates creating a simple Flask application, containerizing it using Docker, pushing the code to GitHub, and uploading the Docker image to Docker Hub.

## 🚀 Project Structure

devops-assignment2/
│
├── app.py
├── requirements.txt
├── Dockerfile
└── README.md

## 📌 Steps Performed

### 1️⃣ Create Flask Application
A simple Flask app was created that returns a welcome message on `/`.

### 2️⃣ Create Dockerfile
A Dockerfile was written to:
- Use Python base image
- Install Flask
- Copy application files
- Expose port 5000
- Run the application

### 3️⃣ Build Docker Image
docker build -t flask-demo:latest .

### 4️⃣ Test Docker Image Locally
docker run --rm -p 5000:5000 flask-demo:latest

### 5️⃣ Tag Image for Docker Hub
docker tag flask-demo:latest purvashinde21/flask-demo:latest

### 6️⃣ Push Image to Docker Hub
docker push purvashinde21/flask-demo:latest

### 7️⃣ Push Code to GitHub
git add .
git commit -m "Added Flask app, Dockerfile, and project setup"
git push origin main

## 🔗 Repository & Image Links

### ✔ GitHub Repository
https://github.com/PurvaShinde21/devops-assignment2

### ✔ Docker Hub Image
https://hub.docker.com/r/purvashinde21/flask-demo

## 👍 Author
Purva Shinde
