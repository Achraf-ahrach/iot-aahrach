# iot-aahrach

This project is part of the **Inception-of-Things** training.

It uses:

- **K3d** to create a local Kubernetes cluster.
- **Argo CD** to deploy an application using Git (GitOps).

## 📦 App Information

This app uses a Docker image from [DockerHub](https://hub.docker.com/r/wil42/playground).

- Image: `wil42/playground`
- Version: `v1`
- Port: `8888`

## 📁 Files

- `deployment.yaml`: Deploys the app to the Kubernetes `dev` namespace.
- `service.yaml`: Exposes the app inside the cluster on port 80.

## ✅ How It Works

1. Argo CD reads the files from this GitHub repository.
2. It applies the `deployment.yaml` and `service.yaml` files.
3. The app runs in the **dev** namespace.

## 👨‍💻 Author

Achraf Ahrach (`aahrach`)
