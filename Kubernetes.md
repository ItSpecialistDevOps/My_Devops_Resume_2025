# Kubernetes – Detailed Expertise

## Skills
- Wrote Kubernetes manifests for Deployments, Services, and ConfigMaps.
- Managed resources with `kubectl` (pods, services, namespaces).
- Implemented rolling updates and rollbacks.
- Configured Horizontal Pod Autoscaler (HPA).
- Deployed workloads on AKS with Persistent Volumes.

## Example Deployment Manifest
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: todo-app
spec:
  replicas: 3
  selector:
    matchLabels:
      app: todo-app
  template:
    metadata:
      labels:
        app: todo-app
    spec:
      containers:
        - name: todo-app
          image: itspecialistdevops/todo-app:latest
          ports:
            - containerPort: 80
