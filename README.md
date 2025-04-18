# 🚀 NestJS Boilerplate – Docker + Kubernetes Ready

This is a minimal NestJS application setup, ready to be containerized with Docker and deployed to a Kubernetes cluster.

---

## 🧱 Tech Stack

- NestJS
- Docker
- Kubernetes
- Node.js

---

## 📁 Project Structure

. ├── src/ │ ├── app.controller.ts │ ├── app.module.ts │ └── main.ts ├── Dockerfile ├── .dockerignore ├── k8s/ │ ├── deployment.yaml │ └── service.yaml ├── package.json └── README.md


## Setup Instructions

### Install Dependencies

To get started, first install the necessary dependencies for the application:

```bash
npm install

npm run start

The application should now be running on http://localhost:3000.
```


### Run in k8s cluster

To run in K8s cluster


```bash
kubectl create -f deployment.yaml
kubectl create -f service.yaml

minikube service nestjs-k8s --url #to get the url
