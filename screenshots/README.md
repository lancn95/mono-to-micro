# Screenshots
To help review your infrastructure, please include the following screenshots in this directory::

## Deployment Pipeline
* DockerHub showing containers that you have pushed
* GitHub repository’s settings showing your Travis webhook (can be found in Settings - Webhook)
* Travis CI showing a successful build and deploy job

## Kubernetes
CICD:
![Alt text](ci.png)
![Alt text](hubs.png)
* To verify Kubernetes pods are deployed properly
```bash
kubectl get pods
```
![Alt text](pods.png)
* To verify Kubernetes services are properly set up
```bash
kubectl describe services
```
![Alt text](svc1.png)
![Alt text](svc2.png)
![Alt text](svc3.png)

* To verify that you have horizontal scaling set against CPU usage
```bash
kubectl describe hpa
```
![Alt text](HPA1.png)
* To verify that you have set up logging with a backend application
```bash
kubectl logs {pod_name}
```
![Alt text](logs.png)
