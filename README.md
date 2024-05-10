# Kubernetes example of PHP-FPM + NGINX !
This example was created to help beginners on Kubernetes (like me).
Fell free to improve that as strart for studies.

## How to run that ?
```
kind create cluster --name phpfpm-nginx --config=kind/kind.yaml 
```

```
kubectl cluster-info --context kind-phpfpm-nginx
```

```
kubectl apply -f .
```

## How to test that ?
Execute in your browser:
http://localhost:30000

AFTER wait some seconds, if everything is ok you will see:
![alt text](https://i.ibb.co/NZ88dtG/Screenshot-2024-05-09-at-21-23-38.png)

*if you are in mac your windows don't forget to share the base folder to use volumes:
(docker desktop preferences ->resource->file sharing)