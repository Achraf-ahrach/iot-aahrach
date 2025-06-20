# iot-aahrach

Minimal K3d + Argo CD project for deploying a containerized app using GitOps.

# iot-aahrach

This project is part of the **Inception-of-Things** curriculum.

It uses:

- **K3d**: to run a local Kubernetes cluster inside Docker
- **Argo CD**: to deploy an app automatically using Git (GitOps)

## 📦 Application

We are deploying the app `wil42/playground` from DockerHub.

- It runs on port `8888`
- It has two versions: `v1` and `v2`

The app is deployed to the **dev** namespace using Argo CD.

## 📁 Project Structure

iot-aahrach/

├── app/

│ └── deployment.yaml # Kubernetes manifest for the app

└── app-of-app.yaml # Argo CD Application definition

## 🚀 How It Works

1. Argo CD watches this GitHub repo.
2. When you update `deployment.yaml`, Argo CD updates the app in your cluster.

## ✅ Goal

- Understand GitOps with Argo CD
- Deploy and update apps using Git and Kubernetes

## 🔗 Docker Image

Using Wil's image:
https://hub.docker.com/r/wil42/playground

## 👨‍💻 Author

Ashraf Ahrash (aahrach)
