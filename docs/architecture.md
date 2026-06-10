# Current Architecture

## Cluster

- Host: platform.airvault.io
- OS: Debian 12
- Kubernetes: v1.33.6+k3s1
- Runtime: containerd

## Nodes

- 1 Control Plane Node

## Installed Components

- CoreDNS
- Metrics Server
- Local Path Provisioner

## Storage

Default StorageClass:

- local-path

## Current Workloads

- nginx deployment

## Target Architecture

Internet
  |
Cloudflare DNS
  |
Ingress-NGINX
  |
Namespaces
  |
Applications

Shared Platform Services

- ArgoCD
- Prometheus
- Grafana
- Loki
