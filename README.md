 

# CI/CD Deployment with Flask and Docker

This project demonstrates a complete CI/CD pipeline using **GitHub Actions**, **Docker**, and **Flask**.

## Overview
- A simple **Flask web application** with a basic UI and API endpoint.
- **GitHub Actions** for automating the build and deployment process.
- **Containerization** of the Flask app using Docker.
- **Deployment to Docker Hub** for easy distribution and usage.

## Workflow
1. **Develop**: Flask app is created and maintained in this repository.
2. **Containerize**: A `Dockerfile` is used to package the application.
3. **Automate**: GitHub Actions build and push the Docker image to Docker Hub.
4. **Deploy**: The containerized application is ready to be pulled and run anywhere.

## Technologies Used
- **Flask** (for building the web application)
- **Docker** (for containerization)
- **GitHub Actions** (for CI/CD automation)
- **Docker Hub** (for hosting container images)

## How to Run Locally
```sh
# Clone the repository
git clone https://github.com/Vinay-kanuku/CICD_wrokflow.git
cd  CICD_wrokflow

# Install dependencies
pip install -r requirements.txt

# Run the Flask app
python app.py
```

## Running with Docker
```sh
# Build the Docker image
docker build -t my-flask-app .

# Run the container
docker run -p 5000:5000 my-flask-app
```

## CI/CD Pipeline
GitHub Actions automatically builds and pushes the Docker image to Docker Hub on every push to `main`.

