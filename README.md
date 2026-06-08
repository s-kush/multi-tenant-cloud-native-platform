# Multi-Tenant Cloud Native Platform

A hands-on platform engineering project built on K3s to demonstrate:

- Kubernetes Administration
- GitOps with ArgoCD
- Infrastructure Automation
- Monitoring and Observability
- Multi-Tenant Platform Design
- Reliability Engineering

## Current Status

- K3s Cluster: Running
- Kubernetes Version: v1.33.6+k3s1
- Runtime: containerd
- Storage: local-path
- Monitoring: metrics-server

## Planned Components

- ingress-nginx
- ArgoCD
- Prometheus
- Grafana
- Loki
- Multi-Tenant Workloads
- Backup and Recovery
- Multi-Node Expansion

## Repository Structure

docs/         Project documentation
k8s/          Kubernetes manifests
gitops/       ArgoCD applications
monitoring/   Monitoring stack
platform/     Platform design
notes/        Operational notes
