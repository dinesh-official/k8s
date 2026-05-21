# k8s


k8s-platform-engineering/
│
├── README.md
├── .gitignore
├── LICENSE
│
├── docs/
│   ├── architecture/
│   │   ├── aws/
│   │   ├── hybrid-infra/
│   │   ├── ai-platform/
│   │   ├── gitops/
│   │   ├── monitoring/
│   │   └── networking/
│   │
│   ├── linux/
│   │   ├── ubuntu/
│   │   ├── systemd/
│   │   ├── storage/
│   │   ├── networking/
│   │   ├── ssh/
│   │   ├── security/
│   │   └── troubleshooting/
│   │
│   ├── docker/
│   │   ├── basics/
│   │   ├── dockerfiles/
│   │   ├── compose/
│   │   ├── volumes/
│   │   ├── networking/
│   │   ├── registry/
│   │   ├── optimization/
│   │   └── troubleshooting/
│   │
│   ├── kubernetes/
│   │   ├── basics/
│   │   │   ├── pods/
│   │   │   ├── deployments/
│   │   │   ├── services/
│   │   │   ├── ingress/
│   │   │   ├── configmaps/
│   │   │   ├── secrets/
│   │   │   ├── namespaces/
│   │   │   ├── jobs/
│   │   │   ├── cronjobs/
│   │   │   ├── daemonsets/
│   │   │   ├── statefulsets/
│   │   │   └── storage/
│   │   │
│   │   ├── networking/
│   │   │   ├── cni/
│   │   │   ├── ingress/
│   │   │   ├── dns/
│   │   │   ├── loadbalancer/
│   │   │   ├── metallb/
│   │   │   └── networkpolicy/
│   │   │
│   │   ├── security/
│   │   │   ├── rbac/
│   │   │   ├── serviceaccounts/
│   │   │   ├── secrets/
│   │   │   ├── policies/
│   │   │   ├── falco/
│   │   │   ├── trivy/
│   │   │   └── cert-manager/
│   │   │
│   │   ├── storage/
│   │   │   ├── pv/
│   │   │   ├── pvc/
│   │   │   ├── storageclass/
│   │   │   ├── longhorn/
│   │   │   └── backup/
│   │   │
│   │   ├── helm/
│   │   │   ├── charts/
│   │   │   ├── values/
│   │   │   ├── templates/
│   │   │   └── custom-chart/
│   │   │
│   │   ├── gitops/
│   │   │   ├── argocd/
│   │   │   ├── applications/
│   │   │   ├── appsets/
│   │   │   ├── sync-policies/
│   │   │   └── workflows/
│   │   │
│   │   ├── monitoring/
│   │   │   ├── prometheus/
│   │   │   ├── grafana/
│   │   │   ├── loki/
│   │   │   ├── alertmanager/
│   │   │   ├── exporters/
│   │   │   └── dashboards/
│   │   │
│   │   ├── traefik/
│   │   │   ├── ingressroute/
│   │   │   ├── middleware/
│   │   │   ├── tls/
│   │   │   ├── letsencrypt/
│   │   │   └── rate-limit/
│   │   │
│   │   ├── k3s/
│   │   │   ├── master/
│   │   │   ├── worker/
│   │   │   ├── gpu-worker/
│   │   │   ├── backup/
│   │   │   ├── restore/
│   │   │   └── upgrades/
│   │   │
│   │   ├── gpu/
│   │   │   ├── nvidia-runtime/
│   │   │   ├── cuda/
│   │   │   ├── gpu-scheduling/
│   │   │   ├── device-plugin/
│   │   │   ├── ollama/
│   │   │   ├── vllm/
│   │   │   └── pytorch/
│   │   │
│   │   ├── ai-infra/
│   │   │   ├── langchain/
│   │   │   ├── langgraph/
│   │   │   ├── rag/
│   │   │   ├── qdrant/
│   │   │   ├── embeddings/
│   │   │   ├── ai-agents/
│   │   │   └── inference/
│   │   │
│   │   └── troubleshooting/
│   │       ├── crashloopbackoff/
│   │       ├── imagepullbackoff/
│   │       ├── dns/
│   │       ├── ingress/
│   │       ├── gpu/
│   │       ├── storage/
│   │       ├── networking/
│   │       └── performance/
│   │
│   ├── aws/
│   │   ├── ec2/
│   │   ├── ecs/
│   │   ├── eks/
│   │   ├── ecr/
│   │   ├── alb/
│   │   ├── vpc/
│   │   ├── route53/
│   │   ├── iam/
│   │   ├── cloudwatch/
│   │   ├── rds/
│   │   ├── elasticache/
│   │   └── security/
│   │
│   ├── cicd/
│   │   ├── github-actions/
│   │   ├── pipelines/
│   │   ├── ghcr/
│   │   ├── deployments/
│   │   └── automation/
│   │
│   └── sre/
│       ├── observability/
│       ├── incident-response/
│       ├── scaling/
│       ├── disaster-recovery/
│       ├── backup/
│       ├── alerting/
│       └── postmortem/
│
├── manifests/
│   ├── nginx/
│   ├── qdrant/
│   ├── ollama/
│   ├── argocd/
│   ├── traefik/
│   ├── prometheus/
│   ├── grafana/
│   ├── loki/
│   ├── cert-manager/
│   ├── longhorn/
│   └── ai-agents/
│
├── labs/
│   ├── k3s-cluster-setup/
│   ├── gpu-worker-setup/
│   ├── argocd-install/
│   ├── traefik-ingress/
│   ├── monitoring-stack/
│   ├── ai-infra-deployment/
│   └── disaster-recovery/
│
├── scripts/
│   ├── setup/
│   ├── backup/
│   ├── restore/
│   ├── monitoring/
│   ├── automation/
│   └── troubleshooting/
│
├── cheatsheets/
│   ├── kubectl.md
│   ├── helm.md
│   ├── docker.md
│   ├── linux.md
│   ├── aws.md
│   └── git.md
│
├── diagrams/
│   ├── aws/
│   ├── kubernetes/
│   ├── ai-platform/
│   ├── networking/
│   └── monitoring/
│
├── projects/
│   ├── hybrid-k3s-cluster/
│   ├── ai-platform/
│   ├── gitops-platform/
│   └── monitoring-stack/
│
└── templates/
    ├── deployment.yaml
    ├── service.yaml
    ├── ingress.yaml
    ├── pvc.yaml
    ├── configmap.yaml
    ├── secret.yaml
    ├── daemonset.yaml
    └── statefulset.yaml
