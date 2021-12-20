# Kubernetes

## Basics of K8s
- K8s is an orchestration system to deploy and manage containers

### Components
- Powerful API
- Allows for decoupling of services
- Easy to add new containers to run new services
- K8s allows for breaking a monilithic application into multiple smaller services that communicate with each other
- The transient nature of smaller services also allows for decoupling
- Each aspect of the traditional application is replaced with a dedicated, but transient, microservice or agent. To join these agents, or their replacements together, we use services

### Challenges
- Building and managing containers at scale and creating distributed applications is challenging
- Steps:
    - Decide on a CI/CD pipeline (Jenkins, Helm, etc.)
    - Select infrastructure to run the containers
    - Roll out updates and terminate containers when not needed
    - Need a reliable network that will join containers as they get spin up
    - Need a storage infrastructure which provides and keeps or recycles the storage in a seamless manner

### Architecture
- Architecture: [Architecture diagram](files/bbfvycyedbcb-Kubernetes_Architecture.png)
- Every node running a container has a kubelet and kube-proxy
- K8s consists of control plane (*cp*) nodes and worker nodes
    - The cp runs an API server, a scheduler, various controllers and a storage system to keep the state of the cluster, container settings, and the networking configuration
- Kubernetes exposes an API via the API server. You can communicate with the API using a local client called kubectl or you can write your own client and use curl commands
- Each node in the cluster runs two processes: a kubelet, which is often a systemd process, not a container, and kube-proxy
- Kube-proxy: creates and manages networking rules to expose the container on the network to other containers or the outside world
- Kubelet: receives requests to run the containers, manages any resources necessary and works with the container engine to manage them on the local node



