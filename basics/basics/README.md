
# Kubernetes Command Syntax
```
kubectl [ACTION] [RESOURCE] [NAME] [FLAGS]
```

=> Action  
```
What you want to do, like get, create 

Actions
  - get
  - create
  - apply
  - edit


```

| Action          | Description                                | Example                                                       |
| --------------- | ------------------------------------------ | ------------------------------------------------------------- |
| `get`           | List Kubernetes resources                  | `kubectl get pods`                                            |
| `describe`      | Show detailed information about a resource | `kubectl describe pod nginx-pod`                              |
| `apply`         | Create or update resources using YAML      | `kubectl apply -f deployment.yaml`                            |
| `create`        | Create a new resource                      | `kubectl create namespace dhangpt`                            |
| `delete`        | Remove a resource                          | `kubectl delete pod nginx-pod`                                |
| `edit`          | Edit live Kubernetes resource              | `kubectl edit deployment nginx`                               |
| `logs`          | View container logs                        | `kubectl logs nginx-pod`                                      |
| `exec`          | Execute command inside container           | `kubectl exec -it nginx-pod -- bash`                          |
| `scale`         | Increase or decrease replicas              | `kubectl scale deployment nginx --replicas=3`                 |
| `rollout`       | Manage deployment rollout operations       | `kubectl rollout restart deployment nginx`                    |
| `expose`        | Expose deployment/service                  | `kubectl expose deployment nginx --port=80`                   |
| `port-forward`  | Forward local port to pod/service          | `kubectl port-forward pod/nginx-pod 8080:80`                  |
| `top`           | Show CPU and memory usage                  | `kubectl top pods`                                            |
| `cordon`        | Disable scheduling on node                 | `kubectl cordon node1`                                        |
| `uncordon`      | Enable scheduling on node                  | `kubectl uncordon node1`                                      |
| `drain`         | Safely remove workloads from node          | `kubectl drain node1 --ignore-daemonsets`                     |
| `label`         | Add labels to resources                    | `kubectl label pod nginx env=prod`                            |
| `annotate`      | Add annotations/metadata                   | `kubectl annotate pod nginx owner=dinesh`                     |
| `cp`            | Copy files between local and pod           | `kubectl cp file.txt nginx-pod:/tmp/`                         |
| `api-resources` | List all Kubernetes resource types         | `kubectl api-resources`                                       |
| `api-versions`  | List supported API versions                | `kubectl api-versions`                                        |
| `cluster-info`  | Show cluster information                   | `kubectl cluster-info`                                        |
| `config`        | Manage kubeconfig settings                 | `kubectl config get-contexts`                                 |
| `auth`          | Check permissions/access                   | `kubectl auth can-i create pods`                              |
| `taint`         | Apply taints to nodes                      | `kubectl taint nodes node1 gpu=true:NoSchedule`               |
| `patch`         | Apply partial updates                      | `kubectl patch deployment nginx -p '{"spec":{"replicas":2}}'` |
| `replace`       | Replace entire resource configuration      | `kubectl replace -f deployment.yaml`                          |
| `wait`          | Wait for resource condition                | `kubectl wait --for=condition=ready pod/nginx-pod`            |
| `explain`       | Explain Kubernetes YAML fields             | `kubectl explain deployment`                                  |
| `version`       | Show Kubernetes client/server version      | `kubectl version`                                             |


=> Resource
```


```



| Part     | Meaning             | Example    |
| -------- | ------------------- | ---------- |
| kubectl  | Kubernetes CLI tool | kubectl    |
| ACTION   | what you want to do | get        |
| RESOURCE | object type         | pods       |
| NAME     | specific object     | nginx-pod  |
| FLAGS    | extra options       | -n dhangpt |
