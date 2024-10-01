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
API Server
Controller Manager
Scheduler
ETCD
![Screenshot from 2024-10-01 12-31-26](https://github.com/user-attachments/assets/fe92e8e6-4e77-4ec6-b677-ba6d5daf30c2)









