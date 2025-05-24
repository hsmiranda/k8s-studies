# How is to work

1. Apply the postgres-pv.yaml with command so checking the status is ok.:
```
kubectl apply -f postgres-pv.yaml
kubectl get pv
```

2. Apply the postgres-pvc.yaml with command so checking the status is ok.:
```
kubectl apply -f postgres-pvc.yaml
kubectl get pv
```

3. Apply the postgres-configmap.yaml with command so checking the status is ok.:
```
kubectl apply -f postgres-configmap.yaml
kubectl 
``` 

4. Apply the postgres-secrets.yaml with command so checking the status is ok, the password is admin:
```
kubectl apply -f postgres-secrets.yaml
kubectl 
``` 

5. Apply the postgres-statefulset.yaml with command so checking the status is ok, the password is admin:
```
kubectl apply -f postgres-statefulset.yaml
kubectl get stateful
``` 

6. Apply the postgres-svc.yaml with command so checking the status is ok:
```
kubectl apply -f postgres-svc.yaml
kubectl get svc
``` 

7. Execute port-forward for check connect:
```
kubectl port-forward svc/postgres 5432:5432
```
8. Connect in your database with client.
