## 4- Kubernetes Tools and Installations
Before moving on to the installation of Kubernetes tools, let's first examine what these tools are used for:
**a) kubeadm:** is a tool that helps you to set up Kubernetes Cluster.
**b) kubelet:** It is a tool that helps to register Node to API server and can run on any Node.
**c) kubectl:** It is a command line tool with which you can control Kubernetes Cluster.
Now, let's install these tools by entering the following command in the terminal:
```
yum install kubeadm kubectl kubelet -y
```
After the installations are completed successfully, let's start the first kubelet tool and activate it:
```
systemctl start kubelet
systemctl enable kubelet
```
Then we need to disable the swap by entering the ``swapoff -a`` command in the terminal.
-> After successfully completing the above operations, you can proceed to the last step of our training, where we will perform operations with other kubernetes tools.