
default
  - This is the default namespace on the launch, so every pod and other resources will be landed on this Namespace

kube-node-lease
  - Kubernetes nodes send heartbeat updates roughly every 10 seconds to confirm they are alive.
  - Example heartbeat
    - Node name
    - Current timestamp (last seen time)

kube-public
  - Inside the Kubernetes cluster, even unauthenticated users can read it
  -  Anyone can read resources in a namespace in entire cluster, but nobody can delete or edit them.

kube-system
  - kube-system is the Kubernetes namespace that runs all the core cluster components like networking, DNS, scheduling, and 
  control plane services needed for the cluster to function.

