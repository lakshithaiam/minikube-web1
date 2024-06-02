
MinikubeWeb is a project aimed at deploying a simple website using Minikube and Kubernetes. It showcases the process of containerizing a web application, deploying it on a local Kubernetes cluster, and exposing it for access.

## Getting Started

To get started with MinikubeWeb, follow the instructions below:

### Prerequisites

- [Minikube](https://minikube.sigs.k8s.io/docs/start/) installed on your local machine
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/) installed on your local machine
- [Docker](https://docs.docker.com/get-docker/) installed on your local machine

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/minikube-web.git


Navigate to the project directory:
cd minikube-web

Build the Docker image:
docker build -t my-website:1.0 .


Deployment


Start Minikube:
minikube start

Apply the Kubernetes deployment:
kubectl apply -f website-deployment.yaml

Expose the deployment:
kubectl expose deployment website-deployment --type=NodePort --port=80

Access the website:
minikube service website-deployment

