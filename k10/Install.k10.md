Source: https://docs.kasten.io/latest/install/aws/aws.html
# Install k10

```bash
kubectl create namespace kasten-io
helm install k10 kasten/k10 --namespace=kasten-io 
# or with create namespace
helm install k10 kasten/k10 --namespace=kasten-io --create-namespace
```

## Validating the install
```bash
kubectl get pods --namespace kasten-io --watch
```