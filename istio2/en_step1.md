### 1) Istio Setup
In our previous tutorial, we examined what **Istio** is and why it is used. Now we will look at how to install Istio on Kubernetes. If you're ready, let's get started 🚀

First, enter the following command to install the latest release of Istioctl on the machine that was charged to you:
````
curl -L https://istio.io/downloadIstio | sh -
````
Additionally, if you want to install a specific version, you can use the following command:
````
curl -L https://istio.io/downloadIstio | ISTIO_VERSION=1.3.0 sh -
````

Now that we have installed Istioctl, enter the following command to install Istio with the demo profile we will use in the Traffic Management example:
````
istioctl manifest apply --set profile=demo
````
The above command will install all the components in the demo profile to the Kubernetes cluster. You can examine the installed components with the following command:
````
kubectl get all -n istio-system
````

--> Now that we have successfully completed the Istio installation, we can move on to the next step, traffic management with Istio.