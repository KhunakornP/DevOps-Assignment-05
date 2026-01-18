# DevOps-Assignment-05
Classwork for DevSecOps 2026-01219493 course from Kasetsart University

This repository uses the web-application from [Kubernetes Crash Course for Absolute Beginners](https://www.youtube.com/watch?v=s_o8dwzRlu4&t=2s), the link to the docker image can be found [here](https://hub.docker.com/repository/docker/nanajanashia/k8s-demo-app)


## Pre-requisites
- A hosted/self-managed kubenetes cluster
    - Capable of handling a load balancer

## How to run
Run all the setup scripts (in order)
```
kubeclt apply -f mongo-secret.yaml
```

```
kubeclt apply -f mongo-config.yaml
```

```
kubeclt apply -f mongo.yaml
```

```
kubeclt apply -f webapp.yaml
```

Run ```kubeclt get pods``` and check the IP to connect to the application