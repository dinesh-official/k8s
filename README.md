# k8s

~~~
K8s/
├── README.md
├── cheatsheets/
│   ├── kubectl.md
│   ├── helm.md
│   ├── argocd.md
│   ├── kustomize.md
│   ├── troubleshooting.md
│   └── networking.md
│
├── templates/
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── ingress.yaml
│   ├── pvc.yaml
│   ├── configmap.yaml
│   ├── secret.yaml
│   ├── daemonset.yaml
│   ├── statefulset.yaml
│   ├── hpa.yaml
│   └── cronjob.yaml
│
├── kubernetes/
│   ├── basics/
│   │   ├── pods/
│   │   ├── deployments/
│   │   ├── replicasets/
│   │   ├── services/
│   │   ├── ingress/
│   │   ├── namespaces/
│   │   ├── configmaps/
│   │   ├── secrets/
│   │   ├── labels-selectors/
│   │   ├── annotations/
│   │   ├── jobs/
│   │   ├── cronjobs/
│   │   ├── daemonsets/
│   │   ├── statefulsets/
│   │   ├── taints-tolerations/
│   │   ├── affinity/
│   │   ├── resource-limits/
│   │   ├── probes/
│   │   └── init-containers/
│   │
│   ├── networking/
│   │   ├── clusterip/
│   │   ├── nodeport/
│   │   ├── loadbalancer/
│   │   ├── ingress/
│   │   ├── ingress-controller/
│   │   ├── cni/
│   │   ├── dns/
│   │   ├── networkpolicy/
│   │   ├── metallb/
│   │   └── service-mesh/
│   │
│   ├── storage/
│   │   ├── pv/
│   │   ├── pvc/
│   │   ├── storageclass/
│   │   ├── csi/
│   │   ├── longhorn/
│   │   ├── snapshots/
│   │   └── backups/
│   │
│   ├── security/
│   │   ├── rbac/
│   │   ├── serviceaccounts/
│   │   ├── secrets-management/
│   │   ├── network-policies/
│   │   ├── pod-security/
│   │   ├── image-security/
│   │   ├── trivy/
│   │   ├── falco/
│   │   └── cert-manager/
│   │
│   ├── scaling/
│   │   ├── hpa/
│   │   ├── vpa/
│   │   ├── cluster-autoscaler/
│   │   └── karpenter/
│   │
│   ├── observability/
│   │   ├── prometheus/
│   │   ├── grafana/
│   │   ├── loki/
│   │   ├── tempo/
│   │   ├── jaeger/
│   │   ├── alertmanager/
│   │   ├── metrics-server/
│   │   └── dashboards/
│   │
│   ├── ingress/
│   │   ├── traefik/
│   │   ├── nginx-ingress/
│   │   ├── ingressroute/
│   │   ├── middleware/
│   │   ├── tls/
│   │   ├── letsencrypt/
│   │   └── rate-limit/
│   │
│   ├── helm/
│   │   ├── basics/
│   │   ├── charts/
│   │   ├── values/
│   │   ├── templating/
│   │   ├── dependencies/
│   │   ├── repositories/
│   │   ├── helmfile/
│   │   └── custom-charts/
│   │
│   ├── gitops/
│   │   ├── argocd/
│   │   ├── applications/
│   │   ├── app-of-apps/
│   │   ├── applicationsets/
│   │   ├── sync-policy/
│   │   ├── rollback/
│   │   ├── kustomize/
│   │   └── fluxcd/
│   │
│   ├── operators/
│   │   ├── operator-sdk/
│   │   ├── custom-controllers/
│   │   ├── crds/
│   │   └── kube-builder/
│   │
│   ├── runtime/
│   │   ├── containerd/
│   │   ├── cri-o/
│   │   ├── runtimeclass/
│   │   └── gvisor/
│   │
│   ├── gpu/
│   │   ├── nvidia-device-plugin/
│   │   ├── gpu-scheduling/
│   │   ├── cuda/
│   │   ├── gpu-monitoring/
│   │   ├── ollama/
│   │   ├── vllm/
│   │   └── pytorch/
│   │
│   ├── distributions/
│   │   ├── k3s/
│   │   ├── rke2/
│   │   ├── eks/
│   │   ├── aks/
│   │   ├── gke/
│   │   ├── openshift/
│   │   └── microk8s/
│   │
│   ├── cicd/
│   │   ├── github-actions/
│   │   ├── gitlab-ci/
│   │   ├── jenkins/
│   │   ├── image-build/
│   │   ├── deployments/
│   │   └── rollback/
│   │
│   ├── ai-workloads/
│   │   ├── qdrant/
│   │   ├── rag/
│   │   ├── embeddings/
│   │   ├── llm-inference/
│   │   ├── ai-agents/
│   │   ├── langchain/
│   │   └── langgraph/
│   │
│   ├── sre/
│   │   ├── disaster-recovery/
│   │   ├── backup-restore/
│   │   ├── incident-management/
│   │   ├── logging/
│   │   ├── monitoring/
│   │   ├── sla-slo-sli/
│   │   └── performance-tuning/
│   │
│   └── troubleshooting/
│       ├── crashloopbackoff/
│       ├── pending-pods/
│       ├── dns-issues/
│       ├── ingress-issues/
│       ├── pvc-issues/
│       ├── node-notready/
│       ├── imagepullbackoff/
│       ├── oomkilled/
│       ├── certificate-errors/
│       ├── networking/
│       ├── gpu-issues/
│       └── performance/
│
├── manifests/
│   ├── deployments/
│   ├── services/
│   ├── ingress/
│   ├── pvc/
│   ├── configmaps/
│   ├── secrets/
│   ├── helm-values/
│   ├── argocd/
│   ├── monitoring/
│   ├── gpu/
│   └── ai/
│
├── labs/
│   ├── local-cluster/
│   ├── k3s-cluster/
│   ├── argocd-setup/
│   ├── traefik-setup/
│   ├── monitoring-stack/
│   ├── gpu-worker/
│   ├── ai-platform/
│   └── gitops-workflow/
│
├── diagrams/
│   ├── cluster-architecture/
│   ├── gitops-flow/
│   ├── ingress-flow/
│   ├── monitoring-flow/
│   ├── ai-platform/
│   └── networking/
│
└── projects/
    ├── hybrid-k3s-cluster/
    ├── ai-platform/
    ├── monitoring-stack/
    ├── gitops-platform/
    └── gpu-inference-platform/



~~~
