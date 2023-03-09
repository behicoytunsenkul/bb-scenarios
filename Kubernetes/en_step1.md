## 3- How to Install Kubernetes?
  In order for us to install Kubernetes on our system, the Docker application must first be installed on all Centos servers. However, we do not perform any installation process because Docker comes pre-installed on our system.
  >You can get help from our Docker training series for Dokcer installations on your personal device.
  In the first lesson of our Kubernetes training, we will install **kubeadm**, **kubelet** and **kubectl** tools. To install ``curl`` on our system first, enter the following command in the terminal:
```
 yum install curl -y
 ```
 After the ``curl`` installation is completed successfully, we need to add the Kubernetes repository to all servers. To do this, we first need a create a file:
```
 vi /etc/yum.repos.d/kubernetes.repo
```
After creating the file, you can close the file and return to the terminal screen. Now we can start installing the **Kubernetes Tools** we just mentioned.
 
--> You can move on to the next step of our Kubernetes training.