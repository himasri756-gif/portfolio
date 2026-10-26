# portfolio
My personal portfolio  website


## Docker Deployment
This portfolio website is containerized using Docker and Nginx.

- Docker Hub Image: `himasri756/portfolio:1.0`

## Kubernetes Deployment
The portfolio website is deployed locally using Kubernetes with Minikube.

### Kubernetes Resources
- Deployment: `portfolio`
- Service: `portfolio-service`
- Service Type: NodePort
- Container Port: 80
- Status: Running

### Commands Used
```bash
minikube start --driver=docker
kubectl apply -f kubernetes/portfolio.yaml
kubectl get pods
kubectl get services
kubectl get deployments
minikube service portfolio-service --url
```
