### Using Istio
Istio **by-pass** Kubernetes' default network configuration to manage traffic for applications running on kubernetes. It adds its own sidecar proxy containers to the pods of the applications and runs the rules such as network and security that it will define through these proxies.

> **Sidecar Proxy Container:** It is a frequently used concept in microservice architectures and service mesh solutions. Its main purpose is to run the same host environment as the main container and undertake important tasks such as managing, controlling and making the network traffic of the service more secure.

Before starting to use Istio, some configuration adjustments are required. First, enter the following command on your allocated machine:
````
istioctl proxy-status
````
You can follow the instructions below for proxy configuration.

**1)** To get information about cluster configuration for Envoy instance on a particular pod, you can use the following command:
````
istioctl proxy-config cluster <pod-name> [flags]
````
**2)** To get information about the boot configuration for the Envoy instance on a particular pod, you can use the following command:
````
istioctl proxy-config bootstrap <pod-name> [flags]
````
**3)** You can use the following command to get information about the listener configuration for the Envoy instance on a particular pod:
````
istioctl proxy-config listener <pod-name> [flags]
````
**4)** You can use the following command to get information about the route configuration of the Envoy instance on a particular pod:
````
istioctl proxy-config route <pod-name> [flags]
````
**5)** To get information about the end-point configuration for the Envoy instance on a particular pod, you can use the following command:
````
istioctl proxy-config endpoints <pod-name> [flags]
````