# devopslive4.1
Assignmentt 4

# download minikube

curl -LO https://storage.googleapis.com/minikube/releases/latest/minikube-linux-amd64

# install minikube 

sudo install minikube-linux-amd64 /usr/local/bin/minikube


# Start Mini Kube
minikube start --force

# define alieas
alias kubectl="minikube kubectl --"


#  enable dashboard

minikube addons enable dashboard


# enable proxy

minikube kubectl proxy --address='0.0.0.0' --disable-filter=true


# dashboard

![image](https://github.com/sydali/devopslive4.1/assets/449393/c1a94097-94a2-4618-85e5-23b0c7abe9f2)

```


root@dice-devops:/usr/local/bin# minikube  status
minikube
type: Control Plane
host: Running
kubelet: Running
apiserver: Running
kubeconfig: Configured

root@dice-devops:~# kubectl  get nodes
NAME       STATUS   ROLES           AGE   VERSION
minikube   Ready    control-plane   16d   v1.28.3



root@dice-devops:/usr/local/bin# kubectl version
Client Version: v1.28.3
Kustomize Version: v5.0.4-0.20230601165947-6ce0bf390ce3
Unable to connect to the server: net/http: TLS handshake timeout
root@dice-devops:/usr/local/bin# minikube version
minikube version: v1.32.0
commit: 8220a6eb95f0a4d75f7f2d7b14cef975f050512d


```
