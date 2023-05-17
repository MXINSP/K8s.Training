# K8s Training

---
## Docker Commands
* `docker-compose up` 
  * From the same folder where docker-compose.yml is localed
  * To builds, (re)creates, and start containers
* `docker-compose down`
---
## K8s Concepts
* Pod
  - Smallest object of the k8s object model
  - Environment for containers
  - To run a single pod:
    - `kubectl run <POD_NAME> --image=<IMAGE_NAME>`
    - `kubectl run my-nginx --image=nginx:alpine`
  - To view all pods:
    - `kubectl get pods`
  - To expose a container pod outside of the cluster:
    - `kubectl port-forward <POD_NAME> 8080:80`
    - `kubectl apply -f nginx.pod.yml --dry-run=client`
  - To delete a pod:
    - `kubectl delete pod <POD_NAME>`

* Node
  - Master & Worker
* Replica set
* Stateful set
* Daemon set
* Persistent volume
* Ingress
* Service
* Namespace
* Auto-scaler
* Environment variables
* Health check
* Config map
* Deployment
* Label
* Job
* Cron job
* Service

---
## AKS (Azure Kubernetes Service)
* Azure Managed (Control Plane)
  * API Server
  * Scheduler
  * etcd
  * Controller
* Customer Managed
  * Node 1
    * kubelet
    * Runtime
    * kube-proxy
    * Container
  * Node 2
    * ...
  * Node 3
    * ...
---
## Links:
* [Hosting ASP.NET Core images with Docker over HTTPS](https://learn.microsoft.com/en-us/aspnet/core/security/docker-https?view=aspnetcore-7.0)
* [Hosting ASP.NET Core images with Docker Compose over HTTPS](https://learn.microsoft.com/en-us/aspnet/core/security/docker-compose-https?view=aspnetcore-7.0)
* [Compose sample application: ASP.NET with MS SQL server database](https://github.com/docker/awesome-compose/tree/master/aspnet-mssql)
* [Monitoring ASP.NET Fx applications in Windows Docker containers, using Prometheus](https://github.com/dockersamples/aspnet-monitoring)
* [Docker Samples](https://github.com/dockersamples)
