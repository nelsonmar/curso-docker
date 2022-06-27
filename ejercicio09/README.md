# Resolución

Ejecutar:

```
kubectl apply -f deployment.yml
```

Una vez que los pods estén corriendo: 

```
kubectl get pods
kubectl exec -it <nombre_de_un_pod> -- bash
```

Una vez adentro de la aplicación:

```
curl localhost:3000/password
```
