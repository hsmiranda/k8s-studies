# How is to work

1. Apply the mysql-pv.yaml with command so checking the status is ok:
```
kubectl apply -f mysql-pv.yaml
kubectl get pv
```

2. Apply the mysql-pvc.yaml with command so checking the status is ok:
```
kubectl apply -f mysql-pvc.yaml
kubectl get pv
```

3. Apply the mysql-secrets.yaml with command so checking the status is ok, the password is admin:
```
kubectl apply -f mysql-secrets.yaml
kubectl get secrets
``` 

4. Apply the mysql-statefulset.yaml with command so checking the status is ok, the password is admin:
```
kubectl apply -f mysqlostgres-statefulset.yaml
kubectl get stateful
``` 

5. Apply the mysql-svc.yaml with command so checking the status is ok:
```
kubectl apply -f mysql-svc.yaml
kubectl get svc
``` 

6. Execute port-forward for check connect:
```
kubectl port-forward svc/mysql 3306:3306
```

7. Connect in your database with client.
