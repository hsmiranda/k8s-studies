# How is to work

1. Apply the adminer-deployment.yaml with command:
```
kubectl apply -f adminer-deployment.yaml
```

2. Execute adminer-svc.yaml with command:
```
kubectl apply -f adminer-svc.yaml
```

3. Create ingress with command below if ingress not existe:
```
helm upgrade --install ingress-nginx ingress-nginx --repo https://kubernetes.github.io/ingress-nginx --namespace ingress-nginx --create-namespace
```

4. Apply ingress configuration with:
```
kubectl apply -f ingress-controller.yaml
```
