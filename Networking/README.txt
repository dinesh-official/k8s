| Component     | Purpose                  |
| ------------- | ------------------------ |
| Pod Network   | Pod-to-Pod communication |
| Service       | Stable access to Pods    |
| kube-proxy    | Traffic forwarding       |
| CNI Plugin    | Creates networking       |
| DNS           | Service discovery        |
| Ingress       | HTTP routing             |
| NetworkPolicy | Firewall rules           |


pod networking
--------------
    - each pod will have its own ip so if one pod get stop it is difficult to route the traffic 
    - any pod can talk to any pod 

    Issues  
    ------
        Old IP → gone
        New IP → assigned

Service
-------
    - ClusterIP
        - Internal communication inside the cluster 

    - NodePort
        - External access to expose the pod output on the web or any (Exposes app externally via Node IP.)

    - LoadBalancer
        - Cloud load balancer 

    - ExternalName
        - DNS alias




kube-proxy
----------
    - Kube-proxy is an makes virtual networking actualy work 
      Service Ip is an virtual networking and the kube-proxy makes it actualy work
    - kube-proxy runs on every node 

    please refer the arichiture here at res/kube-proxy.jpg  

  User/App
      ↓
  Service IP
  10.96.0.15
      ↓
  kube-proxy
      ↓
  Chooses Pod
      ↓
  10.244.0.5


CNI Plugin
----------

DNS
---
    - Kubernetes automatically creates DNS names.

Ingress
-------

NetworkPolicy
-------------