# Kubernetes Pods

## Aim
Create and run a simple Nginx Pod in Kubernetes.

## What is a Pod?
A Pod is the smallest deployable unit in Kubernetes. It can contain one or more containers.

## YAML File

```yaml
apiVersion: v1
kind: Pod
metadata:
  name: nginx-pod
spec:
  containers:
    - name: nginx-container
      image: nginx
```

## Commands

Create Pod:

```bash
kubectl apply -f pod.yaml
```

View Pods:

```bash
kubectl get pods
```

Describe Pod:

```bash
kubectl describe pod nginx-pod
```

Delete Pod:

```bash
kubectl delete -f pod.yaml
```

## Expected Output

- Pod status should be Running.
- Nginx container should start successfully.

## Interview Questions

1. What is a Pod?
2. Can a Pod contain multiple containers?
3. What happens if a Pod crashes?
4. What is the smallest unit in Kubernetes?