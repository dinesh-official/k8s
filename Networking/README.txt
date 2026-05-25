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
    - Used for an interal communication for eg:- 
    (say for an example if 3 Component of app need to communicat each other but this is hosted in 3 differ nodes hree CNI creates an interface to make an connection )

    - Node ↔ Node networking works
    - Pod ↔ Pod communication works

DNS
----
    - Kubernetes automatically creates DNS names.
    - Kubernetes DNS = system that converts service names into IP addresses inside the cluster
    - Types of DNS names
        - Service name -> ( backend-service )
        - Full DNS name ->  ( backend-service.default.svc.cluster.local )
          

Ingress
-------
    - Ingress is used to access Kubernetes apps using a simple website link (URL).
    - without Ingress the acess url would be IP:30080 → frontend , IP:30081 → backend , IP:30082 → admin
    - with Ingress  ,shop.com → Frontend , api.shop.com → Backend, admin.shop.com  → Admin panel


NetworkPolicy
-------------
    - NetworkPolicy Which Pod can talk to which Pod
    - This is like an security group in AWS SG will work in Vm level and NP will work in pod level 
    