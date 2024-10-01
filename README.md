# kubernetes
Basics of kubernetes

What is kubernetes?
It is an open source container orchestration tool used for multi container deployment.

Why to use kubernrtes?
- For production ready deployment of microservices or small apps.
- Having less failures and downtimes.
- Backups and restores.

Architecture of kubernetes

![Screenshot from 2024-10-01 11-51-31](https://github.com/user-attachments/assets/a1e2c439-c5da-4dce-8aeb-a843d0361926)

API server manages Worker nodes with the help of kubectl on master node
kubelet manages worker node

Group of servers is called as a cluster

Connectipon between clusters is called as CNI network

Difference between node & pod
- Node is server or virtual machine (Collection of pods)
- Pod is the smallest unit of kubernetes which gives an abstraction over docker container.

Minikube
used to manage k8 on local machine

Firstly install docker

To install the latest minikube stable release on x86-64 Linux using binary download:
curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64
sudo install minikube-linux-amd64 /usr/local/bin/minikube && rm minikube-linux-amd64

kubernetes installed

Now install kubectl
sudo snap install kubectl --classic

Components of Kubernetes
API Server (API for kubelet to communicate)
Controller Manager
Scheduler (watches new pods, select worker nodes to run them on)
ETCD (watches & controls worker nodes, correct numer of pods & more)

![Screenshot from 2024-10-01 12-31-26](https://github.com/user-attachments/assets/fe92e8e6-4e77-4ec6-b677-ba6d5daf30c2)

Containers might crash and need to be replaced.
Container scale up and scale down. (auto scaling)
Incomming traffic should be distributed equally. (load balancer)
------------------------------------------------------------
Services like ECS can help.
but in in aws we have to work like that service

Advantages:-
kubernetes configuration is an advantage
can be used with any cloud
Works with docker
free service

kubernetes is like docker-compose for multiple machines

What kubernetes will do?
Create your objects (pods) & manage them
Monitor pods & recreate them scale pods etc
Kubernetes utilizes the provided resources to apply your configuration .

We have to do?
Create the cluster & node instances (worker + master nodes)
setup API server, kubelet & other
Create other cloud provider resources (eg. load balancer, filesystem)

----------------------------------------------------------------------------
Use docker to create images for creatig containers, and kubernetes will manage containers.


















